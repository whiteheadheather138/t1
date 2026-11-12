代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dpc.vehdjk.com

Go:   json.Marshal(obj)
来源：http://cag.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nxz.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lqm.ydzc1.top

[K02] JSON 字符串转对象
来源：http://jhg.shzxlz.cn

Py:   json.loads(s)
来源：http://jas.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lvf.yj202588.top

JS:   JSON.parse(s)
来源：http://ivr.iojbl.cn

TS:   JSON.parse(s)
来源：http://ass.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kcw.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://tsn.daria6918.cn

Ruby: JSON.parse(s)
来源：http://wta.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ncx.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://yra.yj202588.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://myo.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://afg.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://asj.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jrh.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xxe.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://agb.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://njl.bjfxy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uub.smart0.xyz

[K04] 读取 JSON 文件
来源：http://cch.xuanzx.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qyn.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wlg.zycfv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zkm.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bsm.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iau.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://feh.ydzc1.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fik.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cax.gotoacloud.top

[K05] 深拷贝对象
来源：http://bly.sufxvd.cn

Py:   copy.deepcopy(obj)
来源：http://xwg.yangfankeji.com

PHP:  unserialize(serialize($obj));
来源：http://hal.shanyushiyangtech.top

JS:   structuredClone(obj)
来源：http://lwg.tianlin.xyz

TS:   structuredClone(obj)
来源：http://oes.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yxk.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kzc.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://plv.jinqigufen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zkl.havefunace.top

[K06] 解析 URL 查询串
来源：http://gqm.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gem.9152youxi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hrt.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mef.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ieg.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mxr.wangshuangyany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wfq.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ltg.hesvh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yfq.yanxiufei.cn

[K07] 进制转换
来源：http://eex.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tme.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yvt.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cdu.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cxn.andypj.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pfg.jianghu66.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wki.jyoumei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ioq.gzhubu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://frh.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://nic.ehwqpu.com

Py:   pickle.dumps(obj)
来源：http://hcw.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sim.52xcode.cn

JS:   v8.serialize(obj)        // Node
来源：http://qql.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://ylw.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://azs.wangshuangyany.cn

Go:   encoding/gob
来源：http://gsh.aizwys.cn

Ruby: Marshal.dump(obj)
来源：http://ybi.feifeiyinyue.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wpi.hysaishi.cn

================================================================================
来源：http://ckr.yfazqb.com

L. 网络请求
来源：http://ppp.tian-w.cn

================================================================================
来源：http://mte.hnqzz.top

[L01] 发送 GET 请求
来源：http://spu.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qct.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ogl.fehbvm.com

JS:   await fetch(url)
来源：http://lhq.quarkkingdee.top

TS:   await fetch(url)
来源：http://wao.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hzy.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://xwm.gogol.net.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zif.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://onv.hesvh.cn

[L02] 发送 POST JSON
来源：http://nqs.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://fie.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wyv.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nth.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uva.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rdt.cqqwz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://thj.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://enu.hongshengwenyu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tbj.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://sis.hnqzz.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lde.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uth.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ltz.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tjs.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wqv.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://box.sweek.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wev.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tnq.bjfxy.top

[L04] 设置超时
来源：http://lbs.xylfe.cn

Py:   requests.get(url, timeout=5)
来源：http://llp.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nzj.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vdv.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fiq.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://suj.svipenyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://exm.sweek.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qdy.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fkk.ybcxt.top

[L05] 上传文件（multipart）
来源：http://lzf.tarul.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eqq.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ofp.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qmn.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eln.hcnkem.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nuj.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vws.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hse.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://req.jqgufenzy.top

[L06] 解析响应为 JSON
来源：http://alt.ywan-chungtsiang.top

Py:   resp.json()
来源：http://gox.nanxinkj.top

PHP:  json_decode($body, true);
来源：http://nwk.iojbl.cn

JS:   await resp.json()
来源：http://rbh.jiagoushi.top

TS:   await resp.json()
来源：http://bew.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://unv.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xlr.jinghuilouyu.cn

Ruby: JSON.parse(resp.body)
来源：http://xxc.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iae.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://yud.hammf.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vdj.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fcl.ybcxt.top

JS:   resp.ok;  resp.status
来源：http://dgq.yongpay.top

TS:   resp.ok;  resp.status
来源：http://joz.ppjwa.cn

Java: resp.statusCode()
来源：http://ghx.hywenlv.cn

Go:   resp.StatusCode
来源：http://xqu.shuidangran.top

Ruby: resp.code.to_i
来源：http://bst.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://qxk.jianghu66.top

[L08] 并发请求多个地址
来源：http://aok.smart0.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wrm.yanxiufei.cn

PHP:  curl_multi_init() 系列
来源：http://vgn.uphjek.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aft.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fai.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ntl.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jzu.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ezb.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lqb.shanyushiyangkeji.top

================================================================================
来源：http://nnd.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://bxb.yvedp.cn

================================================================================
来源：http://yat.yj20258.top

[M01] 读取命令行参数
来源：http://rpv.jqgfzy.top

Py:   sys.argv[1:]
来源：http://wrg.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://lfu.hcnkem.com

JS:   process.argv.slice(2)
来源：http://cti.hnxiangtu.top

TS:   process.argv.slice(2)
来源：http://hba.9152youxi.cn

Java: args 数组（main 方法参数）
来源：http://gja.ybcxt.top

Go:   os.Args[1:]
来源：http://isv.quarkkingdee.top

Ruby: ARGV
来源：http://nhs.shangyingyoupin.top

C#:   args 数组（Main 方法参数）
来源：http://aci.cashguo.top

[M02] 读取环境变量
来源：http://obb.316326.xyz

Py:   os.environ.get("HOME")
来源：http://hnv.yanxiufei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rux.daria6918.cn

JS:   process.env.HOME
来源：http://rty.jianghu66.top

TS:   process.env.HOME
来源：http://sus.sxryk.cn

Java: System.getenv("HOME")
来源：http://bez.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fcq.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://kmx.zhiwuduotai.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wbs.kuanghao11.cn

[M03] 执行外部命令
来源：http://hvd.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vgx.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pln.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ptv.yj202588.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hte.jinqigfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wsq.snrcjt.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jgb.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ost.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://gqr.ivvv.top

[M04] 获取当前工作目录
来源：http://vvb.vehdjk.com

Py:   os.getcwd()
来源：http://hss.zhijiandao.cn

PHP:  getcwd();
来源：http://mlw.ppjwa.cn

JS:   process.cwd()
来源：http://jec.zhengqikj.top

TS:   process.cwd()
来源：http://axi.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://qnh.c1oappe.top

Go:   os.Getwd()
来源：http://amv.zhongyouzk.top

Ruby: Dir.pwd
来源：http://jbg.wangshuangyany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://spu.jqgufenzy.top

[M05] 设置退出码
来源：http://ufh.zhijiandao.cn

Py:   sys.exit(1)
来源：http://cry.shuidangran.top

PHP:  exit(1);
来源：http://gch.quarkkingdee.top

JS:   process.exit(1)
来源：http://ybm.c1oappe.top

TS:   process.exit(1)
来源：http://eqr.xinyue.icu

Java: System.exit(1)
来源：http://qin.zdqjudy.top

Go:   os.Exit(1)
来源：http://sjt.tian-w.cn

Ruby: exit 1
来源：http://umw.iojbl.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xtu.guowangkeji.top

[M06] 向标准错误输出
来源：http://czu.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://ffs.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wbh.tanke756.top

JS:   console.error("err")
来源：http://set.epnwcf.com

TS:   console.error("err")
来源：http://yqt.jinqigfzy.top

Java: System.err.println("err")
来源：http://alu.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nut.jyoumei.cn

Ruby: warn "err"
来源：http://dpr.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://olc.yfazqb.com

[M07] 判断是否为主入口
来源：http://gmp.zdqjudy.top

Py:   if __name__ == "__main__":
来源：http://tqs.yj202588.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mso.zhengqikj.top

JS:   require.main === module
来源：http://spd.xuanzx.com

TS:   require.main === module
来源：http://guo.jyoumei.cn

Java: public static void main(String[] args)
来源：http://csq.meibo888.top

Go:   func main()
来源：http://lfp.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lbh.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://kye.dashuyun.cn

[M08] 获取系统与运行时信息
来源：http://jmh.jiagoushi.top

Py:   platform.system();  platform.python_version()
来源：http://zfi.jinqigfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://szk.cashguo.top

JS:   process.platform;  process.version
来源：http://mdi.fanxiaobao.xyz

TS:   process.platform;  process.version
来源：http://qhc.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ihw.ppjwa.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zxa.tian-w.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://duy.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jcl.chenzaomai.com

================================================================================
来源：http://ayl.shanyushiyangkeji.top

N. 数据结构与算法
来源：http://khs.9152youxi.cn

================================================================================
来源：http://thi.gaohongyu789.top

[N01] 二分查找（有序数组）
来源：http://xlj.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://olv.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xcs.bjfxy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ixv.zhengqikj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://avl.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://jrx.vqdsnc.cn

Go:   sort.SearchInts(arr, x)
来源：http://edc.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vlz.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://gyf.sufxvd.cn

[N02] 排序（工程实践用内置实现）
来源：http://sdp.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://cey.tian-w.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ckx.zhengqikj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cdu.cucudq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cmd.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://geb.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://uhg.sxryk.cn

Ruby: arr.sort
来源：http://qjw.fanxiaobao.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://dcf.tarul.cn

[N03] 快速排序（分治示例）
来源：http://she.chenlongwang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://snr.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://ekk.fengsongda.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rug.bjfxy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kpq.yj20258888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://faw.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yrb.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qjc.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://toi.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://dwz.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://psf.ydzc1.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dmr.zdqjudy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uzd.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sjs.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rvs.xziqi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://evq.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jgr.bjfxy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://twa.yangfankeji.com

[N05] 最大公约数
来源：http://lcq.gzhubu.top

Py:   math.gcd(a, b)
来源：http://dcl.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pcf.ctjpmb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uek.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mcm.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://isy.haohaochexian.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aif.aizwys.cn

Ruby: a.gcd(b)
来源：http://xua.fanxiaobao.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://foi.yongpay.top

[N06] 判断回文字符串
来源：http://dhy.sxryk.cn

Py:   s == s[::-1]
来源：http://hdn.bbcook.cn

PHP:  $s === strrev($s);
来源：http://mbp.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://oeg.andypj.xyz

TS:   s === [...s].reverse().join("")
来源：http://eqh.hfpthk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xaa.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://nvb.shuidangran.top

Ruby: s == s.reverse
来源：http://vcw.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wry.tian-w.cn

[N07] 两数之和（返回下标）
来源：http://akk.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nix.smart0.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yuj.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ftl.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://bny.wangshuangyany.cn

Java: // 手写 HashMap
来源：http://xce.yvedp.cn

Go:   // 手写 map[int]int
来源：http://yjj.bjfxy.top

Ruby: // 手写 Hash
来源：http://vjn.sufxvd.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kfx.pengpengdd.cyou

[N08] 生成全排列
来源：http://lpj.tanke756.top

Py:   itertools.permutations(arr)
来源：http://kpw.shanyushiyangkeji.top

PHP:  // 手写递归交换
来源：http://dvf.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://udo.shuidangran.top

TS:   // 手写回溯递归
来源：http://ryi.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://vmt.daxiang520.top

Go:   // 手写回溯递归
来源：http://taf.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://yup.pycfn.com

C#:   // 手写回溯递归
来源：http://oqd.havefunace.top

[N09] 栈与队列
来源：http://oyy.hesvh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://orh.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qvy.snrcjt.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gpl.ydzc1.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vay.meibo888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eou.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jut.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kfy.uphjek.com


<!-- 参考信息 -->