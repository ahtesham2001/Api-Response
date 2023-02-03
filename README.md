# Api-Response
        try {             $getServices = Service::where('status', 1)->get();             return $this->respond($getServices, [], true, 'Data Retrieved');         } catch (\Exception $e) {             return $this->respondInternalError($e->getMessage());         }
