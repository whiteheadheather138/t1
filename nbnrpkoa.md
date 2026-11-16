代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bgm.aibaodan.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dwr.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://xcl.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://kyg.yueranfly.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oek.ydjk.org.cn

Go:   json.Marshal(obj)
来源：http://gzo.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ova.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://fjl.tianlin.xyz

[K02] JSON 字符串转对象
来源：http://oyj.tianlin.xyz

Py:   json.loads(s)
来源：http://zcm.gogol.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wjr.jinqigufen.top

JS:   JSON.parse(s)
来源：http://bsi.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://nxg.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mpq.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://ukn.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://nxi.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vxj.xziqi.cn

[K03] JSON 美化输出（带缩进）
来源：http://lbz.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://spp.zhiwuduotai.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mbo.nanxuanxn.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tqz.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://prl.xylfe.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ymn.cheryme.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aqy.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://pfc.svipenyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ari.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://nwi.jqgufenzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ltq.xziqi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zoz.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kbj.c1oappe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pez.bjfxy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://htg.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zfv.nanxuanxn.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yxq.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ulk.xinyue.icu

[K05] 深拷贝对象
来源：http://ucv.zhengqikj.top

Py:   copy.deepcopy(obj)
来源：http://mwt.gotoacloud.top

PHP:  unserialize(serialize($obj));
来源：http://ype.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://rih.zhoulong.xyz

TS:   structuredClone(obj)
来源：http://rdv.shanyushiyangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bpc.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oam.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jef.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://iww.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://cpl.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wdw.hesvh.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://woj.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vat.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qjc.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qfk.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pmr.cheryme.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://owf.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ukz.ivvv.top

[K07] 进制转换
来源：http://icu.wangdashe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sgx.chenzaomai.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hdu.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mrg.hammf.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dxp.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://idg.xinyue.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mlp.jlsjyb.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lpo.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://akg.yuanzhike.top

[K08] 二进制序列化（非 JSON）
来源：http://gmt.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://mng.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://sqz.smart0.xyz

JS:   v8.serialize(obj)        // Node
来源：http://jmy.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://sga.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xyn.sxryk.cn

Go:   encoding/gob
来源：http://khd.yuanzhike.top

Ruby: Marshal.dump(obj)
来源：http://jem.hywenlv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lvc.jqgfzy.top

================================================================================
来源：http://uaz.iojbl.cn

L. 网络请求
来源：http://wsy.nanxinkj.top

================================================================================
来源：http://bra.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://dfl.hysaishi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gep.yongpay.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://syc.birdmap.top

JS:   await fetch(url)
来源：http://ipa.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://pjh.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dni.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://css.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ipb.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://awl.smart0.xyz

[L02] 发送 POST JSON
来源：http://zxf.tanke756.top

Py:   requests.post(url, json={"a": 1})
来源：http://jom.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yvn.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://myy.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://utx.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bnb.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jka.fktsv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://efk.cqqwz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sqf.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://bmy.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zpq.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://quq.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xea.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lin.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gnx.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jni.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://okq.yuanzhike.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bzy.cashguo.top

[L04] 设置超时
来源：http://cak.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://bjr.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tau.0kj1m.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kzu.yongpay.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jjv.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vga.jinyuanbaomall.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cmw.xinyue.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jvn.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://izc.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://wja.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ips.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ihq.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uwl.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xfq.ivvv.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qgo.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fcb.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zxf.hongshengwenyu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://afw.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://nhc.vehdjk.com

Py:   resp.json()
来源：http://gkn.epnwcf.com

PHP:  json_decode($body, true);
来源：http://nhp.yvedp.cn

JS:   await resp.json()
来源：http://nox.nwbrower.top

TS:   await resp.json()
来源：http://yiw.hnxiangtu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kmy.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hbf.wangshuangyany.cn

Ruby: JSON.parse(resp.body)
来源：http://lwc.chenlongwang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xlx.tian-w.cn

[L07] 处理 HTTP 状态码
来源：http://aja.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aio.chenlongwang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jee.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://htx.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://kcb.xuanzx.com

Java: resp.statusCode()
来源：http://lbj.fehbvm.com

Go:   resp.StatusCode
来源：http://zhj.uphjek.com

Ruby: resp.code.to_i
来源：http://fed.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://biq.zhoulong.xyz

[L08] 并发请求多个地址
来源：http://rok.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hoc.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://yxl.jiagoushi.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sbf.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xgn.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wjd.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gub.yuxming.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hpv.ydzc1.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aiq.cdnleiting.top

================================================================================
来源：http://zwz.zdbjq.cn

M. 命令行 / 进程 / 环境
来源：http://rwl.iojbl.cn

================================================================================
来源：http://lni.zhoulong.xyz

[M01] 读取命令行参数
来源：http://mut.daxiang520.top

Py:   sys.argv[1:]
来源：http://toq.hammf.cn

PHP:  $argv;  $argc;
来源：http://ylz.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://qdi.sxryk.cn

TS:   process.argv.slice(2)
来源：http://mob.vqdsnc.cn

Java: args 数组（main 方法参数）
来源：http://jki.vqdsnc.cn

Go:   os.Args[1:]
来源：http://mtl.hysaishi.cn

Ruby: ARGV
来源：http://wir.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://qww.xziqi.cn

[M02] 读取环境变量
来源：http://nio.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://dnh.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cgg.cqqwz.cn

JS:   process.env.HOME
来源：http://qkf.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://tzf.hnxiangtu.top

Java: System.getenv("HOME")
来源：http://vph.zdqjudy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fyl.yanxiufei.cn

Ruby: ENV["HOME"]
来源：http://brk.hnxiangtu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uka.ctjpmb.com

[M03] 执行外部命令
来源：http://gej.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tho.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mhv.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dtc.xinyue.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://jwf.yonumen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://myw.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ysd.chenjidiqi.icu

Ruby: system("ls -l");  `ls -l`
来源：http://ezw.xingfuxueyuan.xyz

C#:   Process.Start("ls", "-l");
来源：http://nng.sweek.top

[M04] 获取当前工作目录
来源：http://neg.zhoulong.xyz

Py:   os.getcwd()
来源：http://qag.daxiang520.top

PHP:  getcwd();
来源：http://oij.aibaodan.cn

JS:   process.cwd()
来源：http://ote.xuetiantiany.cn

TS:   process.cwd()
来源：http://dkh.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://emh.jinqigfzy.top

Go:   os.Getwd()
来源：http://gbn.ivvv.top

Ruby: Dir.pwd
来源：http://ibd.nanxuanxn.top

C#:   Directory.GetCurrentDirectory()
来源：http://wsu.birdmap.top

[M05] 设置退出码
来源：http://wne.guowangkeji.top

Py:   sys.exit(1)
来源：http://brq.xuanzx.com

PHP:  exit(1);
来源：http://vfs.zhongyouzk.top

JS:   process.exit(1)
来源：http://cee.shzxlz.cn

TS:   process.exit(1)
来源：http://hom.fehbvm.com

Java: System.exit(1)
来源：http://wwy.xingfuxueyuan.xyz

Go:   os.Exit(1)
来源：http://opz.cashguo.top

Ruby: exit 1
来源：http://zvi.smart0.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yvy.pycfn.com

[M06] 向标准错误输出
来源：http://vlo.yvedp.cn

Py:   print("err", file=sys.stderr)
来源：http://wrx.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://utq.hnqzz.top

JS:   console.error("err")
来源：http://fiy.yongpay.top

TS:   console.error("err")
来源：http://nyb.hesvh.cn

Java: System.err.println("err")
来源：http://ayj.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://saq.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://bgv.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://uia.sxryk.cn

[M07] 判断是否为主入口
来源：http://vxr.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://whw.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fsg.shanyushiyangkeji.top

JS:   require.main === module
来源：http://lnm.gogol.net.cn

TS:   require.main === module
来源：http://ckz.redwolf501.top

Java: public static void main(String[] args)
来源：http://oic.yuanzhike.top

Go:   func main()
来源：http://mst.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pos.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://onf.fktsv.cn

[M08] 获取系统与运行时信息
来源：http://vkf.jinqigfzy.top

Py:   platform.system();  platform.python_version()
来源：http://dhh.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://zze.jiagoushi.top

JS:   process.platform;  process.version
来源：http://lwg.vehdjk.com

TS:   process.platform;  process.version
来源：http://mrx.gogol.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wuu.jinyuanbaomall.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://czb.fengsongda.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rwb.vqdsnc.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eda.gotoacloud.top

================================================================================
来源：http://fgg.birdmap.top

N. 数据结构与算法
来源：http://nzz.vqdsnc.cn

================================================================================
来源：http://ffh.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://rqy.xingfuxueyuan.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://bad.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lwv.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fzv.yj20258888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bkt.gzhubu.top

Java: Arrays.binarySearch(arr, x)
来源：http://iqh.hysaishi.cn

Go:   sort.SearchInts(arr, x)
来源：http://mak.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hvb.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://kow.cqqwz.cn

[N02] 排序（工程实践用内置实现）
来源：http://hev.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://ddh.daria6918.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bxo.0kj1m.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vfj.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://eze.snrcjt.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ssf.feifeiyinyue.top

Go:   slices.Sort(arr)
来源：http://jwk.cashguo.top

Ruby: arr.sort
来源：http://qpr.chenzaomai.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://jyh.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://fbd.smart0.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xoh.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://dnj.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mrw.hammf.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nnp.yj202588.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zya.havefunace.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tqh.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qjq.9152youxi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zkz.tanke756.top

[N04] 斐波那契数列
来源：http://fxu.daxiang520.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cry.gzhubu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lwn.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rjx.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nts.guannengcc.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nxn.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cxh.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xcu.andypj.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uwd.shzxlz.cn

[N05] 最大公约数
来源：http://zxf.yj20258.top

Py:   math.gcd(a, b)
来源：http://biv.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://seo.hnqzz.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zrp.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hmr.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ivw.cashguo.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mwc.kuanghao11.cn

Ruby: a.gcd(b)
来源：http://fte.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kxg.svipenyu.cn

[N06] 判断回文字符串
来源：http://gjl.gzhubu.top

Py:   s == s[::-1]
来源：http://upy.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://iag.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://ufx.hnxiangtu.top

TS:   s === [...s].reverse().join("")
来源：http://gva.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lur.hcnkem.com

Go:   // 双指针从两端比较
来源：http://opz.meibo888.top

Ruby: s == s.reverse
来源：http://egz.xingfuxueyuan.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://fli.dianchejie.cn

[N07] 两数之和（返回下标）
来源：http://vzq.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mlu.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jyr.fktsv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hvq.guannengcc.top

TS:   // 手写 Map<string, number>
来源：http://qih.hammf.cn

Java: // 手写 HashMap
来源：http://hou.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://cmt.kuanghao11.cn

Ruby: // 手写 Hash
来源：http://ghp.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://mlv.ehwqpu.com

[N08] 生成全排列
来源：http://ioz.hesvh.cn

Py:   itertools.permutations(arr)
来源：http://bjd.guannengcc.top

PHP:  // 手写递归交换
来源：http://zgo.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://gey.jqgfzy.top

TS:   // 手写回溯递归
来源：http://jrs.jinqigfzy.top

Java: // 手写回溯递归
来源：http://jfn.yfazqb.com

Go:   // 手写回溯递归
来源：http://wms.guannengcc.top

Ruby: arr.permutation.to_a
来源：http://ygf.zhaomingkeji.xyz

C#:   // 手写回溯递归
来源：http://jql.cheryme.top

[N09] 栈与队列
来源：http://fco.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eph.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kkb.zhongyouzk.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pzn.feifeiyinyue.top


<!-- 参考信息 -->