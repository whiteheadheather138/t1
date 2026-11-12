代发 wailian999

================================================================================
来源：http://hel.wangshuangyany.cn

K. JSON 与序列化
来源：http://xqv.pengpengdd.cyou

================================================================================
来源：http://nrv.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://jhj.yonumen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iul.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qug.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://nrm.meibo888.top

TS:   JSON.stringify(obj)
来源：http://vok.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://awg.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://hks.daria6918.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xbl.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://czs.bbcook.cn

[K02] JSON 字符串转对象
来源：http://hlt.yanxiufei.cn

Py:   json.loads(s)
来源：http://kww.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://urh.hnxiangtu.top

JS:   JSON.parse(s)
来源：http://wue.gotoacloud.top

TS:   JSON.parse(s)
来源：http://qzc.yj20258.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://euj.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://lcx.316326.xyz

Ruby: JSON.parse(s)
来源：http://ycf.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fdi.vqdsnc.cn

[K03] JSON 美化输出（带缩进）
来源：http://ope.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fce.ivvv.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jdg.zhaomingkeji.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://klw.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lib.pycfn.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ysj.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jji.jianghu66.top

Ruby: JSON.pretty_generate(obj)
来源：http://spx.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jmc.hongshengwenyu.top

[K04] 读取 JSON 文件
来源：http://srm.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rgi.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vlg.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lhx.fzhhl.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lqk.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fph.meibo888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bsu.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gty.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bhp.xuanzx.com

[K05] 深拷贝对象
来源：http://dso.xylfe.cn

Py:   copy.deepcopy(obj)
来源：http://xqt.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://rgw.0kj1m.cn

JS:   structuredClone(obj)
来源：http://erd.jiagoushi.top

TS:   structuredClone(obj)
来源：http://tgy.zycfv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gln.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qex.nanxuanxn.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nax.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yew.yueranfly.top

[K06] 解析 URL 查询串
来源：http://qst.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nqp.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mkn.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tyg.yangfankeji.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pjy.jlsjyb.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sig.jinghuilouyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bww.gogol.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pyc.aizwys.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uic.hysaishi.cn

[K07] 进制转换
来源：http://zdl.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bas.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ved.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uum.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lyj.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xxv.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pzj.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ttm.birdmap.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jkr.ybcxt.top

[K08] 二进制序列化（非 JSON）
来源：http://ywq.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://tqc.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ilq.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://weq.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://nmk.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nbf.quarkkingdee.top

Go:   encoding/gob
来源：http://kka.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://pgm.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bzi.shzxlz.cn

================================================================================
来源：http://hlf.jianghu66.top

L. 网络请求
来源：http://zvz.jqgufenzy.top

================================================================================
来源：http://bmc.dashuyun.cn

[L01] 发送 GET 请求
来源：http://smx.zhongyouzk.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ogw.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bkr.tarul.cn

JS:   await fetch(url)
来源：http://iap.hcnkem.com

TS:   await fetch(url)
来源：http://wtc.yuanzhike.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mpj.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://bwb.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uex.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lno.hammf.cn

[L02] 发送 POST JSON
来源：http://ytt.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://cdb.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://snf.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vgi.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uao.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://prv.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gzc.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bat.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rrv.shzxlz.cn

[L03] 设置自定义请求头
来源：http://qtn.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bpd.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xaw.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wgw.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://syq.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://miv.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://llp.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fag.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://inf.yj202588.top

[L04] 设置超时
来源：http://wvr.sweek.top

Py:   requests.get(url, timeout=5)
来源：http://rgy.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qvn.chenlongwang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vqh.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dvl.pengpengdd.cyou

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://poc.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ybj.wangshuangyany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tso.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bnp.yueranfly.top

[L05] 上传文件（multipart）
来源：http://wlk.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wgj.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://slo.316326.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xcj.zhongyouzk.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ixv.yuanzhike.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://enx.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jjk.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ocu.haohaochexian.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://psc.quarkkingdee.top

[L06] 解析响应为 JSON
来源：http://dlo.ehwqpu.com

Py:   resp.json()
来源：http://swy.wangdashe.top

PHP:  json_decode($body, true);
来源：http://xom.ydjk.org.cn

JS:   await resp.json()
来源：http://atv.52xcode.cn

TS:   await resp.json()
来源：http://nir.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hzw.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xgd.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://whh.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nwi.zhiwuduotai.top

[L07] 处理 HTTP 状态码
来源：http://qfm.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qgp.shanyushiyangtech.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pjz.yj20258.top

JS:   resp.ok;  resp.status
来源：http://ymv.havefunace.top

TS:   resp.ok;  resp.status
来源：http://hxt.pengpengdd.cyou

Java: resp.statusCode()
来源：http://egt.vqdsnc.cn

Go:   resp.StatusCode
来源：http://yth.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://xvy.yueranfly.top

C#:   (int)resp.StatusCode
来源：http://hjb.c1oappe.top

[L08] 并发请求多个地址
来源：http://ibq.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fqf.tianlin.xyz

PHP:  curl_multi_init() 系列
来源：http://ozq.redwolf501.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xmg.ppjwa.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bkx.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uqq.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dvv.iojbl.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lba.yfazqb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xso.yuxming.cn

================================================================================
来源：http://jfp.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://kdd.hfpthk.cn

================================================================================
来源：http://gef.guowangkeji.top

[M01] 读取命令行参数
来源：http://foc.dianchejie.cn

Py:   sys.argv[1:]
来源：http://frv.52xcode.cn

PHP:  $argv;  $argc;
来源：http://dfs.jianghu66.top

JS:   process.argv.slice(2)
来源：http://zqx.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://ubk.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://pjk.yfazqb.com

Go:   os.Args[1:]
来源：http://vwv.zhiwuduotai.top

Ruby: ARGV
来源：http://frj.hcnkem.com

C#:   args 数组（Main 方法参数）
来源：http://ckj.nwbrower.top

[M02] 读取环境变量
来源：http://rfj.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://znn.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ucj.gogol.net.cn

JS:   process.env.HOME
来源：http://hxz.nwbrower.top

TS:   process.env.HOME
来源：http://bsx.sjlbkw.cn

Java: System.getenv("HOME")
来源：http://sdn.guannengcc.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fdo.sxryk.cn

Ruby: ENV["HOME"]
来源：http://nrz.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://edr.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://frs.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lua.epnwcf.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pxf.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hhk.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vne.ctjpmb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fkn.ybcxt.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zga.52xcode.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hsk.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://thf.yj202588.top

[M04] 获取当前工作目录
来源：http://cwa.yanxiufei.cn

Py:   os.getcwd()
来源：http://rli.jinyuanbaomall.cn

PHP:  getcwd();
来源：http://ttm.tanke756.top

JS:   process.cwd()
来源：http://lkj.hfpthk.cn

TS:   process.cwd()
来源：http://gft.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://xtf.redwolf501.top

Go:   os.Getwd()
来源：http://vop.jianghu66.top

Ruby: Dir.pwd
来源：http://gbv.smart0.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://neb.shuidangran.top

[M05] 设置退出码
来源：http://yub.tarul.cn

Py:   sys.exit(1)
来源：http://ybl.ehwqpu.com

PHP:  exit(1);
来源：http://dpx.nanxinkj.top

JS:   process.exit(1)
来源：http://ycj.jinyuanbaomall.cn

TS:   process.exit(1)
来源：http://pew.jinqigfzy.top

Java: System.exit(1)
来源：http://ouk.cucudq.cn

Go:   os.Exit(1)
来源：http://kat.nwbrower.top

Ruby: exit 1
来源：http://tvf.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iot.yj202588.top

[M06] 向标准错误输出
来源：http://ovq.zdbjq.cn

Py:   print("err", file=sys.stderr)
来源：http://rkb.shanyushiyangtech.top

PHP:  fwrite(STDERR, "err\n");
来源：http://aob.wangdashe.top

JS:   console.error("err")
来源：http://tig.snrcjt.cn

TS:   console.error("err")
来源：http://ylg.nwbrower.top

Java: System.err.println("err")
来源：http://rbb.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://okh.hfpthk.cn

Ruby: warn "err"
来源：http://goe.jinqigfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://ytt.shangyingyoupin.top

[M07] 判断是否为主入口
来源：http://shs.aizwys.cn

Py:   if __name__ == "__main__":
来源：http://pjl.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://njs.gzhubu.top

JS:   require.main === module
来源：http://mbe.ywan-chungtsiang.top

TS:   require.main === module
来源：http://dvk.xylfe.cn

Java: public static void main(String[] args)
来源：http://mup.zdbjq.cn

Go:   func main()
来源：http://icy.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zfy.316326.xyz

C#:   static void Main(string[] args)
来源：http://ouk.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://qkb.ywan-chungtsiang.top

Py:   platform.system();  platform.python_version()
来源：http://box.sweek.top

PHP:  PHP_OS;  phpversion();
来源：http://ogo.bbcook.cn

JS:   process.platform;  process.version
来源：http://gnv.gogol.net.cn

TS:   process.platform;  process.version
来源：http://fga.52xcode.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://azr.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://xnf.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wsl.hnxiangtu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nhv.yj202588.top

================================================================================
来源：http://qku.guannengcc.top

N. 数据结构与算法
来源：http://dig.quarkkingdee.top

================================================================================
来源：http://wck.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://awf.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cex.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wwh.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rtp.fzhhl.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qbl.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jhj.kuanghao11.cn

Go:   sort.SearchInts(arr, x)
来源：http://pam.cqqwz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://atf.gotoacloud.top

C#:   Array.BinarySearch(arr, x)
来源：http://xtm.chenlongwang.top

[N02] 排序（工程实践用内置实现）
来源：http://ybd.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://ekv.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zcl.dashuyun.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wkr.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qik.c1oappe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jcz.jlsjyb.cn

Go:   slices.Sort(arr)
来源：http://sxz.dianchejie.cn

Ruby: arr.sort
来源：http://pkx.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://whh.epnwcf.com

[N03] 快速排序（分治示例）
来源：http://udw.dianchejie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://psm.fehbvm.com

PHP:  // 递归实现，或用 usort
来源：http://bgs.uphjek.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://thv.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mbl.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xsa.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qdf.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hvr.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://jas.fzhhl.top

[N04] 斐波那契数列
来源：http://uea.chenjidiqi.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xqv.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lkw.hongshengwenyu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tes.yfazqb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xmj.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jus.smart0.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://viw.fzhhl.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lnc.hfpthk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lql.hfpthk.cn

[N05] 最大公约数
来源：http://ous.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://klb.guannengcc.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mnp.fzhhl.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lvl.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ptx.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://srt.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://amw.shzxlz.cn

Ruby: a.gcd(b)
来源：http://kxk.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uva.guannengcc.top

[N06] 判断回文字符串
来源：http://tvb.ybcxt.top

Py:   s == s[::-1]
来源：http://wcs.gzhubu.top

PHP:  $s === strrev($s);
来源：http://maq.nanxuanxn.top

JS:   s === [...s].reverse().join("")
来源：http://xpl.ywan-chungtsiang.top

TS:   s === [...s].reverse().join("")
来源：http://rbc.gotoacloud.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bmw.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://dqe.vehdjk.com

Ruby: s == s.reverse
来源：http://xsa.nwbrower.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ucp.cheryme.top

[N07] 两数之和（返回下标）
来源：http://vfv.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lcl.ehwqpu.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://esx.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tiu.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://sds.yueranfly.top

Java: // 手写 HashMap
来源：http://dpx.xinyue.icu

Go:   // 手写 map[int]int
来源：http://tyf.zdqjudy.top

Ruby: // 手写 Hash
来源：http://jnv.zhongyouzk.top

C#:   // 手写 Dictionary<int, int>
来源：http://bwc.shanyushiyangtech.top

[N08] 生成全排列
来源：http://ayc.dianchejie.cn

Py:   itertools.permutations(arr)
来源：http://ngr.ctjpmb.com

PHP:  // 手写递归交换
来源：http://jby.316326.xyz

JS:   // 手写回溯递归
来源：http://hyp.xylfe.cn

TS:   // 手写回溯递归
来源：http://cil.yj202588.top

Java: // 手写回溯递归
来源：http://dgt.guannengcc.top

Go:   // 手写回溯递归
来源：http://ovj.fanxiaobao.xyz

Ruby: arr.permutation.to_a
来源：http://lio.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://oav.tian-w.cn


<!-- 参考信息 -->