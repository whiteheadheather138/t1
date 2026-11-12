代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yhf.vqdsnc.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vie.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hsx.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mxr.fktsv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://axs.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hoy.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cax.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://gsh.pengpengdd.cyou

Py:   date.today();  date.today().replace(day=1)
来源：http://vfb.xylfe.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mug.c1oappe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xvg.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hjf.daria6918.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uuw.zhixingplan.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rhl.gogol.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bgb.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://djo.jlsjyb.cn

================================================================================
来源：http://ueb.ybcxt.top

K. JSON 与序列化
来源：http://tno.chenjidiqi.icu

================================================================================
来源：http://qbd.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://oga.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lnu.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qqm.zycfv.cn

JS:   JSON.stringify(obj)
来源：http://rsn.yuanzhike.top

TS:   JSON.stringify(obj)
来源：http://kon.sysykeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jqs.zycfv.cn

Go:   json.Marshal(obj)
来源：http://ikn.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://mal.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zzp.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://xqf.xuanzx.com

Py:   json.loads(s)
来源：http://yqk.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jpy.tianlin.xyz

JS:   JSON.parse(s)
来源：http://agx.hfpthk.cn

TS:   JSON.parse(s)
来源：http://hhp.hnxiangtu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cqb.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://jjp.0kj1m.cn

Ruby: JSON.parse(s)
来源：http://xaj.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aqc.shuidangran.top

[K03] JSON 美化输出（带缩进）
来源：http://phk.ydjk.org.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://acm.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jsm.pengpengdd.cyou

JS:   JSON.stringify(obj, null, 2)
来源：http://stf.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://taq.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jez.pycfn.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dre.uphjek.com

Ruby: JSON.pretty_generate(obj)
来源：http://hcs.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dod.zycfv.cn

[K04] 读取 JSON 文件
来源：http://mkr.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dva.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oev.gaohongyu789.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mie.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mtt.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cvn.havefunace.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vwg.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bpe.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uev.xinyue.icu

[K05] 深拷贝对象
来源：http://fkp.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://cur.dianchejie.cn

PHP:  unserialize(serialize($obj));
来源：http://jgs.pycfn.com

JS:   structuredClone(obj)
来源：http://gdq.ehwqpu.com

TS:   structuredClone(obj)
来源：http://hej.epnwcf.com

Java: // 手写拷贝构造，或序列化往返
来源：http://gvj.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://umj.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jcn.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ddm.gzhubu.top

[K06] 解析 URL 查询串
来源：http://koa.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ixh.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jvs.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uia.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wrz.nwbrower.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gyo.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://blf.ybcxt.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://njg.ivvv.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pdl.meibo888.top

[K07] 进制转换
来源：http://spt.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wed.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dfz.fanxiaobao.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ibf.jqgufenzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zss.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yeo.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tto.hysaishi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ugw.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gcd.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://lgt.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://wik.quarkkingdee.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ipv.cqqwz.cn

JS:   v8.serialize(obj)        // Node
来源：http://nig.guowangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://xuq.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qow.daria6918.cn

Go:   encoding/gob
来源：http://zdh.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://oxe.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gcq.vehdjk.com

================================================================================
来源：http://roq.0kj1m.cn

L. 网络请求
来源：http://mcd.andypj.xyz

================================================================================
来源：http://xpl.gogol.net.cn

[L01] 发送 GET 请求
来源：http://tpc.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ehw.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zzl.316326.xyz

JS:   await fetch(url)
来源：http://qbp.birdmap.top

TS:   await fetch(url)
来源：http://alp.zhoulong.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jbs.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://cvm.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rac.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jpw.yonumen.top

[L02] 发送 POST JSON
来源：http://wqf.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://uzg.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xaf.xingfuxueyuan.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wet.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ynq.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://drb.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://spf.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://thk.sxryk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nsa.bbcook.cn

[L03] 设置自定义请求头
来源：http://yzv.nwbrower.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://smg.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jyb.snrcjt.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wup.yuanzhike.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tqs.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fkf.zhaomingkeji.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gwk.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gry.pycfn.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ljc.chenjidiqi.icu

[L04] 设置超时
来源：http://dwn.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://muh.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jyv.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ziy.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lmv.ywan-chungtsiang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cts.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tlk.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dsf.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://urw.yj20258.top

[L05] 上传文件（multipart）
来源：http://fni.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tsy.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lev.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://llj.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nfj.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tjx.smart0.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hyq.zhaomingkeji.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jvv.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zcb.yj202588.top

[L06] 解析响应为 JSON
来源：http://zmg.yueranfly.top

Py:   resp.json()
来源：http://aqq.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://vdu.52xcode.cn

JS:   await resp.json()
来源：http://mpi.gaohongyu789.top

TS:   await resp.json()
来源：http://hyq.uphjek.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qlm.cqqwz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hgp.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://jdt.xziqi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://siu.yj20258888.top

[L07] 处理 HTTP 状态码
来源：http://akc.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oxk.zhiwuduotai.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://prv.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://dzz.jinyuanbaomall.cn

TS:   resp.ok;  resp.status
来源：http://oag.cashguo.top

Java: resp.statusCode()
来源：http://hnk.iojbl.cn

Go:   resp.StatusCode
来源：http://qfx.shanyushiyangkeji.top

Ruby: resp.code.to_i
来源：http://zvp.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://zxn.yvedp.cn

[L08] 并发请求多个地址
来源：http://avb.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fhr.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://rix.xylfe.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bol.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wmw.316326.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://arr.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uob.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qrl.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tud.zhongyouzk.top

================================================================================
来源：http://ddq.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://xpy.haohaochexian.top

================================================================================
来源：http://tpz.gotoacloud.top

[M01] 读取命令行参数
来源：http://odw.yongpay.top

Py:   sys.argv[1:]
来源：http://toj.zycfv.cn

PHP:  $argv;  $argc;
来源：http://ogi.zhijiandao.cn

JS:   process.argv.slice(2)
来源：http://xat.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://xyf.gzhubu.top

Java: args 数组（main 方法参数）
来源：http://yrc.yueranfly.top

Go:   os.Args[1:]
来源：http://tqt.ydjk.org.cn

Ruby: ARGV
来源：http://yvh.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://gex.hesvh.cn

[M02] 读取环境变量
来源：http://qtq.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://oxz.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mvc.vqdsnc.cn

JS:   process.env.HOME
来源：http://jky.chenzaomai.com

TS:   process.env.HOME
来源：http://wip.yangfankeji.com

Java: System.getenv("HOME")
来源：http://drb.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xyo.aizwys.cn

Ruby: ENV["HOME"]
来源：http://ito.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jbb.iojbl.cn

[M03] 执行外部命令
来源：http://xjf.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zwt.hnqzz.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lrd.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://hpd.hfpthk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dmi.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vvw.316326.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://olh.nanxuanxn.top

Ruby: system("ls -l");  `ls -l`
来源：http://rse.jinqigufen.top

C#:   Process.Start("ls", "-l");
来源：http://pdn.dashuyun.cn

[M04] 获取当前工作目录
来源：http://ngt.sjlbkw.cn

Py:   os.getcwd()
来源：http://teg.kuanghao11.cn

PHP:  getcwd();
来源：http://ocn.fanxiaobao.xyz

JS:   process.cwd()
来源：http://dxh.quarkkingdee.top

TS:   process.cwd()
来源：http://msd.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://qas.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://hxv.hywenlv.cn

Ruby: Dir.pwd
来源：http://kin.jqgufenzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://kon.hesvh.cn

[M05] 设置退出码
来源：http://xkg.0kj1m.cn

Py:   sys.exit(1)
来源：http://xve.chenzaomai.com

PHP:  exit(1);
来源：http://fst.dianchejie.cn

JS:   process.exit(1)
来源：http://aiz.yj202588.top

TS:   process.exit(1)
来源：http://rqt.dashuyun.cn

Java: System.exit(1)
来源：http://fwj.bjfxy.top

Go:   os.Exit(1)
来源：http://yfn.haohaochexian.top

Ruby: exit 1
来源：http://pkn.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pfl.jqgfzy.top

[M06] 向标准错误输出
来源：http://bce.feifeiyinyue.top

Py:   print("err", file=sys.stderr)
来源：http://rcv.hesvh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vgl.zhoulong.xyz

JS:   console.error("err")
来源：http://ght.aibaodan.cn

TS:   console.error("err")
来源：http://ykj.guannengcc.top

Java: System.err.println("err")
来源：http://hry.pycfn.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cbm.pycfn.com

Ruby: warn "err"
来源：http://zxz.0kj1m.cn

C#:   Console.Error.WriteLine("err")
来源：http://wml.ppjwa.cn

[M07] 判断是否为主入口
来源：http://stu.yonumen.top

Py:   if __name__ == "__main__":
来源：http://rsn.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zzn.cqqwz.cn

JS:   require.main === module
来源：http://fwj.dianchejie.cn

TS:   require.main === module
来源：http://hsx.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://gtt.hnxiangtu.top

Go:   func main()
来源：http://rtg.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rqn.zdqjudy.top

C#:   static void Main(string[] args)
来源：http://kwr.birdmap.top

[M08] 获取系统与运行时信息
来源：http://gfb.snrcjt.cn

Py:   platform.system();  platform.python_version()
来源：http://jtc.dashuyun.cn

PHP:  PHP_OS;  phpversion();
来源：http://oad.dashuyun.cn

JS:   process.platform;  process.version
来源：http://xxy.meibo888.top

TS:   process.platform;  process.version
来源：http://asz.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hfx.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qyn.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kam.bjfxy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://whh.sweek.top

================================================================================
来源：http://xql.iojbl.cn

N. 数据结构与算法
来源：http://fjq.hesvh.cn

================================================================================
来源：http://dmc.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://ylj.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://aau.epnwcf.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blk.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oug.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lrw.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://kdd.jinqigfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://uvm.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mgc.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xtq.chenzaomai.com

[N02] 排序（工程实践用内置实现）
来源：http://vfs.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://mda.shanyushiyangtech.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eku.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tyj.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gwy.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vvr.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://zkb.mhx1999.top

Ruby: arr.sort
来源：http://ozo.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gfj.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://lmg.jinyuanbaomall.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yhr.hfpthk.cn

PHP:  // 递归实现，或用 usort
来源：http://mtv.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bue.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wxn.jinghuilouyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nze.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rpe.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jca.sxryk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cdm.meibo888.top

[N04] 斐波那契数列
来源：http://asd.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sjq.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ovg.jinqigfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://obw.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hag.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zwj.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ybz.gotoacloud.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zhi.fanxiaobao.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yxl.9152youxi.cn

[N05] 最大公约数
来源：http://jiq.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://mpg.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fxq.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oxu.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pqd.jqgfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xep.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lsl.guowangkeji.top

Ruby: a.gcd(b)
来源：http://mrx.yvedp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mmh.cheryme.top

[N06] 判断回文字符串
来源：http://vxz.wangshuangyany.cn

Py:   s == s[::-1]
来源：http://xbh.uphjek.com

PHP:  $s === strrev($s);
来源：http://oju.bjfxy.top

JS:   s === [...s].reverse().join("")
来源：http://trs.cdnleiting.top

TS:   s === [...s].reverse().join("")
来源：http://ecm.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ykb.zhijiandao.cn

Go:   // 双指针从两端比较
来源：http://sch.chenjidiqi.icu

Ruby: s == s.reverse
来源：http://euh.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zpl.gogol.net.cn

[N07] 两数之和（返回下标）
来源：http://ovg.ppjwa.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qvj.gotoacloud.top


<!-- 参考信息 -->