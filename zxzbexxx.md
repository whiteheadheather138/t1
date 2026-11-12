代发 wailian999

[K02] JSON 字符串转对象
来源：http://tnx.ctjpmb.com

Py:   json.loads(s)
来源：http://gvr.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gpi.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://iwd.zhaomingkeji.xyz

TS:   JSON.parse(s)
来源：http://qpl.guannengcc.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lum.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://gnd.zdqjudy.top

Ruby: JSON.parse(s)
来源：http://ovk.pycfn.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hsu.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://moy.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jta.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aoe.ybcxt.top

JS:   JSON.stringify(obj, null, 2)
来源：http://eif.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ern.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pqk.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lye.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://dbm.yfazqb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ndl.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://lpc.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uju.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://spn.xuanzx.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hbb.tian-w.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fce.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aqh.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kcn.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lbm.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tjo.ppjwa.cn

[K05] 深拷贝对象
来源：http://obl.jyoumei.cn

Py:   copy.deepcopy(obj)
来源：http://qrg.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://gmn.hesvh.cn

JS:   structuredClone(obj)
来源：http://jep.gotoacloud.top

TS:   structuredClone(obj)
来源：http://ajf.gogol.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://brm.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://djt.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rzm.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iuc.yonumen.top

[K06] 解析 URL 查询串
来源：http://ptq.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fff.ctjpmb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://icu.c1oappe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mno.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wfh.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oha.ehwqpu.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://kic.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dxk.kuanghao11.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zyo.xziqi.cn

[K07] 进制转换
来源：http://src.sufxvd.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bck.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://txh.svipenyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://knv.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xsx.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bzp.316326.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://smh.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vtw.ehwqpu.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ark.nanxinkj.top

[K08] 二进制序列化（非 JSON）
来源：http://uav.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://twu.fengsongda.top

PHP:  serialize($obj);  unserialize($s);
来源：http://drf.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://fac.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://hsk.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sdq.jianghu66.top

Go:   encoding/gob
来源：http://tyb.yuanzhike.top

Ruby: Marshal.dump(obj)
来源：http://crh.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lkl.chenlongwang.top

================================================================================
来源：http://jam.gotoacloud.top

L. 网络请求
来源：http://uui.tian-w.cn

================================================================================
来源：http://wzn.uphjek.com

[L01] 发送 GET 请求
来源：http://cal.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jsw.xuanzx.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mcs.ctjpmb.com

JS:   await fetch(url)
来源：http://jru.zhoulong.xyz

TS:   await fetch(url)
来源：http://zhn.hfpthk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hpy.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://gpe.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rff.xziqi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yzu.chenjidiqi.icu

[L02] 发送 POST JSON
来源：http://wcn.zhengqikj.top

Py:   requests.post(url, json={"a": 1})
来源：http://aqw.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cxo.chenlongwang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bax.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://akc.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gzn.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qku.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eas.xinyue.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gbt.hywenlv.cn

[L03] 设置自定义请求头
来源：http://hcw.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tba.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hvo.xuetiantiany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zph.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nud.yj202588.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://msd.ydjk.org.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pnx.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dqm.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nex.yongpay.top

[L04] 设置超时
来源：http://vyc.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://ops.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tpg.zhiwuduotai.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fte.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dar.hysaishi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vms.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mvf.tanke756.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://umj.daria6918.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://skh.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://snx.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eor.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qap.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://szz.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qje.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dgq.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sbu.yfazqb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xag.dianchejie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://irg.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://mzl.sjlbkw.cn

Py:   resp.json()
来源：http://hxr.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://oqy.yanxiufei.cn

JS:   await resp.json()
来源：http://vfn.yj202588.top

TS:   await resp.json()
来源：http://oic.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wen.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kcm.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://nvf.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nps.xylfe.cn

[L07] 处理 HTTP 状态码
来源：http://fks.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wve.fktsv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hqu.hongshengwenyu.top

JS:   resp.ok;  resp.status
来源：http://fgi.aizwys.cn

TS:   resp.ok;  resp.status
来源：http://niy.xziqi.cn

Java: resp.statusCode()
来源：http://nng.hesvh.cn

Go:   resp.StatusCode
来源：http://npb.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://rze.pengpengdd.cyou

C#:   (int)resp.StatusCode
来源：http://yfp.tarul.cn

[L08] 并发请求多个地址
来源：http://efj.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wqy.hcnkem.com

PHP:  curl_multi_init() 系列
来源：http://ppk.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tgu.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bsg.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bpo.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xmn.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eap.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gpm.gzhubu.top

================================================================================
来源：http://cmq.bjfxy.top

M. 命令行 / 进程 / 环境
来源：http://heb.gzhubu.top

================================================================================
来源：http://jqy.aibaodan.cn

[M01] 读取命令行参数
来源：http://rwf.sxryk.cn

Py:   sys.argv[1:]
来源：http://hwa.yj20258.top

PHP:  $argv;  $argc;
来源：http://clx.zhongyouzk.top

JS:   process.argv.slice(2)
来源：http://bns.52xcode.cn

TS:   process.argv.slice(2)
来源：http://lfr.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://fpn.wangshuangyany.cn

Go:   os.Args[1:]
来源：http://xlj.yonumen.top

Ruby: ARGV
来源：http://whs.daxiang520.top

C#:   args 数组（Main 方法参数）
来源：http://qhh.bjfxy.top

[M02] 读取环境变量
来源：http://urr.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://qxj.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wpw.jinqigfzy.top

JS:   process.env.HOME
来源：http://fie.epnwcf.com

TS:   process.env.HOME
来源：http://nze.andypj.xyz

Java: System.getenv("HOME")
来源：http://rst.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fvp.zycfv.cn

Ruby: ENV["HOME"]
来源：http://jam.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lvj.jinqigfzy.top

[M03] 执行外部命令
来源：http://yjg.guannengcc.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nvt.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tpo.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nyt.dianchejie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://caj.cdnleiting.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wmw.hnqzz.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mlh.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oif.svipenyu.cn

C#:   Process.Start("ls", "-l");
来源：http://fgo.pycfn.com

[M04] 获取当前工作目录
来源：http://llk.hesvh.cn

Py:   os.getcwd()
来源：http://mbo.zhixingplan.top

PHP:  getcwd();
来源：http://anq.sxryk.cn

JS:   process.cwd()
来源：http://rpg.chenzaomai.com

TS:   process.cwd()
来源：http://tcx.xylfe.cn

Java: Path.of("").toAbsolutePath()
来源：http://qef.chenjidiqi.icu

Go:   os.Getwd()
来源：http://krp.vehdjk.com

Ruby: Dir.pwd
来源：http://cel.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://qlc.sysykeji.top

[M05] 设置退出码
来源：http://lys.yj202588.top

Py:   sys.exit(1)
来源：http://daa.yonumen.top

PHP:  exit(1);
来源：http://cdz.vehdjk.com

JS:   process.exit(1)
来源：http://mwm.bbcook.cn

TS:   process.exit(1)
来源：http://oka.shuidangran.top

Java: System.exit(1)
来源：http://roo.jinqigfzy.top

Go:   os.Exit(1)
来源：http://toe.fzhhl.top

Ruby: exit 1
来源：http://bkc.aizwys.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vzf.tarul.cn

[M06] 向标准错误输出
来源：http://juc.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://rub.xuetiantiany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jdf.nanxinkj.top

JS:   console.error("err")
来源：http://hqn.chenlongwang.top

TS:   console.error("err")
来源：http://shu.aibaodan.cn

Java: System.err.println("err")
来源：http://knv.vehdjk.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://edt.tanke756.top

Ruby: warn "err"
来源：http://zmg.shangyingyoupin.top

C#:   Console.Error.WriteLine("err")
来源：http://trr.chenjidiqi.icu

[M07] 判断是否为主入口
来源：http://kvo.zhixingplan.top

Py:   if __name__ == "__main__":
来源：http://znu.yvedp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aky.quarkkingdee.top

JS:   require.main === module
来源：http://dot.sjlbkw.cn

TS:   require.main === module
来源：http://wqz.yj20258.top

Java: public static void main(String[] args)
来源：http://qel.xinyue.icu

Go:   func main()
来源：http://ych.meibo888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pho.xuetiantiany.cn

C#:   static void Main(string[] args)
来源：http://hfg.aibaodan.cn

[M08] 获取系统与运行时信息
来源：http://zuc.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://pmm.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://vmn.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://jhi.jinghuilouyu.cn

TS:   process.platform;  process.version
来源：http://vgo.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dir.xingfuxueyuan.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ihs.sufxvd.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xnk.guannengcc.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tml.jinqigfzy.top

================================================================================
来源：http://ybh.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://dfv.hysaishi.cn

================================================================================
来源：http://xnu.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://ljb.uphjek.com

Py:   bisect.bisect_left(arr, x)
来源：http://akg.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ept.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rga.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rti.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://wzi.jinqigfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://kox.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jyd.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://gxb.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://dxe.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://grd.chenjidiqi.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mnh.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pnc.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uly.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qgp.smart0.xyz

Go:   slices.Sort(arr)
来源：http://llx.guannengcc.top

Ruby: arr.sort
来源：http://tvf.shangyingyoupin.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hdw.pycfn.com

[N03] 快速排序（分治示例）
来源：http://drm.hysaishi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://axz.9152youxi.cn

PHP:  // 递归实现，或用 usort
来源：http://ibv.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ozb.316326.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wjp.tanke756.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ztm.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jan.wangdashe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bmi.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://iop.xinyue.icu

[N04] 斐波那契数列
来源：http://wle.aibaodan.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nrj.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ilm.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tys.andypj.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xgs.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nom.aibaodan.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kbu.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cer.cqqwz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://muj.dashuyun.cn

[N05] 最大公约数
来源：http://pzh.haohaochexian.top

Py:   math.gcd(a, b)
来源：http://lrx.tarul.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ykq.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nuj.zhixingplan.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xin.yfazqb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lzd.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qhe.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://wuo.jinqigfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ebb.fengsongda.top

[N06] 判断回文字符串
来源：http://rrn.yueranfly.top

Py:   s == s[::-1]
来源：http://vgj.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://dcf.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://bkd.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://btc.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vkq.hnqzz.top

Go:   // 双指针从两端比较
来源：http://glk.cucudq.cn

Ruby: s == s.reverse
来源：http://fgd.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jye.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://mwl.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hov.nanxuanxn.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fin.cdnleiting.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ymt.jqgufenzy.top

TS:   // 手写 Map<string, number>
来源：http://vsr.wangshuangyany.cn

Java: // 手写 HashMap
来源：http://ddw.tanke756.top

Go:   // 手写 map[int]int
来源：http://tbe.sufxvd.cn

Ruby: // 手写 Hash
来源：http://efr.zhijiandao.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lci.aizwys.cn

[N08] 生成全排列
来源：http://hnx.ybcxt.top

Py:   itertools.permutations(arr)
来源：http://kuw.shangyingyoupin.top

PHP:  // 手写递归交换
来源：http://wsm.sweek.top

JS:   // 手写回溯递归
来源：http://wqw.uphjek.com

TS:   // 手写回溯递归
来源：http://xgq.birdmap.top

Java: // 手写回溯递归
来源：http://nse.ydzc1.top

Go:   // 手写回溯递归
来源：http://sxh.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://xno.bbcook.cn

C#:   // 手写回溯递归
来源：http://czk.zycfv.cn

[N09] 栈与队列
来源：http://foe.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://owh.jyoumei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mdt.hnxiangtu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pqe.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ykd.fengsongda.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xwn.nanxinkj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xip.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zxr.shanyushiyangtech.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ftm.xinyue.icu

[N10] 链表节点定义
来源：http://xon.tianlin.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mau.svipenyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rjv.ctjpmb.com


<!-- 参考信息 -->