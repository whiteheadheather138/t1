代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jmq.jinghuilouyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vbc.jianghu66.top

[J09] 时区处理
来源：http://hoi.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sga.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oyw.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bzj.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ncz.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jen.hcnkem.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lhe.daxiang520.top

Ruby: Time.now.getlocal("+08:00")
来源：http://oih.hcnkem.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://stk.yj20258888.top

[J10] 取今天 / 本月第一天
来源：http://qun.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://flp.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bho.fanxiaobao.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hjf.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cqs.chenlongwang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cjq.hongshengwenyu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zae.xylfe.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tsd.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uph.meibo888.top

================================================================================
来源：http://oju.bbcook.cn

K. JSON 与序列化
来源：http://ogu.wangshuangyany.cn

================================================================================
来源：http://zja.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://bld.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zen.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://poj.hcnkem.com

JS:   JSON.stringify(obj)
来源：http://brt.jiagoushi.top

TS:   JSON.stringify(obj)
来源：http://nyb.haohaochexian.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://azm.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://yvl.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qmj.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://xgi.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://qrv.chenlongwang.top

Py:   json.loads(s)
来源：http://dhb.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xcm.pycfn.com

JS:   JSON.parse(s)
来源：http://nui.nwbrower.top

TS:   JSON.parse(s)
来源：http://ijs.gotoacloud.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dev.zhijiandao.cn

Go:   json.Unmarshal(data, &v)
来源：http://fow.hesvh.cn

Ruby: JSON.parse(s)
来源：http://qxb.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uce.xuanzx.com

[K03] JSON 美化输出（带缩进）
来源：http://fbn.shangyingyoupin.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://faa.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bmi.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uar.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xvx.aibaodan.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://joo.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yrb.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://ydn.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yme.xylfe.cn

[K04] 读取 JSON 文件
来源：http://edn.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://drk.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cpf.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qmc.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ges.jlsjyb.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lnu.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kav.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://vna.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qdq.sjlbkw.cn

[K05] 深拷贝对象
来源：http://isw.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://lbm.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://hic.nanxinkj.top

JS:   structuredClone(obj)
来源：http://krg.guowangkeji.top

TS:   structuredClone(obj)
来源：http://wyq.svipenyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qvx.bbcook.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cfa.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ayr.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hct.chenzaomai.com

[K06] 解析 URL 查询串
来源：http://jet.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xxw.nwbrower.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vym.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gjs.chenzaomai.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xkh.ivvv.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qsn.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zwo.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lkt.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zaz.svipenyu.cn

[K07] 进制转换
来源：http://tok.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iri.zhongyouzk.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bmo.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zmm.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cqp.pycfn.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yvb.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rkn.jinqigfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bpv.yvedp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://stg.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://rsr.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://vpc.vqdsnc.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jmk.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://ylu.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://xkv.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jxl.xuetiantiany.cn

Go:   encoding/gob
来源：http://pfa.chenzaomai.com

Ruby: Marshal.dump(obj)
来源：http://mzj.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xva.dianchejie.cn

================================================================================
来源：http://ugf.aibaodan.cn

L. 网络请求
来源：http://tyn.cheryme.top

================================================================================
来源：http://czm.jqgufenzy.top

[L01] 发送 GET 请求
来源：http://vuw.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rdu.zdbjq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cfa.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://mpv.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://gjr.xuetiantiany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rmf.svipenyu.cn

Go:   resp, err := http.Get(url)
来源：http://vlg.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://oep.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hkt.ivvv.top

[L02] 发送 POST JSON
来源：http://cpg.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://ylg.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lxx.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aik.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ten.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xwq.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qeq.xinyue.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wzg.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lhw.cucudq.cn

[L03] 设置自定义请求头
来源：http://qpe.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://prv.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jlq.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cma.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wlo.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bvm.ppjwa.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://taa.aibaodan.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xsi.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://odu.ehwqpu.com

[L04] 设置超时
来源：http://xmd.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://exx.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ugs.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hlj.yuxming.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wpq.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://has.kuanghao11.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ano.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rls.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://akf.fehbvm.com

[L05] 上传文件（multipart）
来源：http://bam.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://etp.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wlj.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tud.yuanzhike.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oac.svipenyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vgq.bjfxy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fiq.zhoulong.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gfp.daxiang520.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bzf.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://vek.tianlin.xyz

Py:   resp.json()
来源：http://ksk.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://fgw.xziqi.cn

JS:   await resp.json()
来源：http://djg.xingfuxueyuan.xyz

TS:   await resp.json()
来源：http://jfv.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ldp.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bjy.shuidangran.top

Ruby: JSON.parse(resp.body)
来源：http://bdu.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://npt.yongpay.top

[L07] 处理 HTTP 状态码
来源：http://ywx.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jal.shuidangran.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uuo.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://yxv.zycfv.cn

TS:   resp.ok;  resp.status
来源：http://fqo.nanxuanxn.top

Java: resp.statusCode()
来源：http://mhg.ppjwa.cn

Go:   resp.StatusCode
来源：http://wec.yj20258888.top

Ruby: resp.code.to_i
来源：http://sdv.yangfankeji.com

C#:   (int)resp.StatusCode
来源：http://upp.gogol.net.cn

[L08] 并发请求多个地址
来源：http://vxq.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pzx.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://ghl.shangyingyoupin.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://evw.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nwv.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xar.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ozd.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uqx.cashguo.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://izc.fanxiaobao.xyz

================================================================================
来源：http://tsy.hongshengwenyu.top

M. 命令行 / 进程 / 环境
来源：http://ect.xingfuxueyuan.xyz

================================================================================
来源：http://umh.xuanzx.com

[M01] 读取命令行参数
来源：http://xwq.hesvh.cn

Py:   sys.argv[1:]
来源：http://nvm.yfazqb.com

PHP:  $argv;  $argc;
来源：http://jbi.52xcode.cn

JS:   process.argv.slice(2)
来源：http://tje.meibo888.top

TS:   process.argv.slice(2)
来源：http://btq.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://ynz.316326.xyz

Go:   os.Args[1:]
来源：http://phd.shzxlz.cn

Ruby: ARGV
来源：http://erj.ctjpmb.com

C#:   args 数组（Main 方法参数）
来源：http://tmv.sxryk.cn

[M02] 读取环境变量
来源：http://qyk.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://xez.ydjk.org.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ayl.bjfxy.top

JS:   process.env.HOME
来源：http://bth.uphjek.com

TS:   process.env.HOME
来源：http://fks.yfazqb.com

Java: System.getenv("HOME")
来源：http://lti.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zih.birdmap.top

Ruby: ENV["HOME"]
来源：http://vvm.hnxiangtu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bgv.ppjwa.cn

[M03] 执行外部命令
来源：http://yew.yuxming.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://trz.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vmz.guannengcc.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jsg.aibaodan.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gts.yj202588.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://syt.shuidangran.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pyu.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://bgz.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://xal.jiagoushi.top

[M04] 获取当前工作目录
来源：http://ltn.zhijiandao.cn

Py:   os.getcwd()
来源：http://ukm.zhixingplan.top

PHP:  getcwd();
来源：http://lla.ybcxt.top

JS:   process.cwd()
来源：http://slk.yuanzhike.top

TS:   process.cwd()
来源：http://tfy.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://cug.pycfn.com

Go:   os.Getwd()
来源：http://rvn.yanxiufei.cn

Ruby: Dir.pwd
来源：http://fye.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kbr.cqqwz.cn

[M05] 设置退出码
来源：http://yge.yueranfly.top

Py:   sys.exit(1)
来源：http://sfn.quarkkingdee.top

PHP:  exit(1);
来源：http://mpq.gaohongyu789.top

JS:   process.exit(1)
来源：http://djp.haohaochexian.top

TS:   process.exit(1)
来源：http://tdi.jlsjyb.cn

Java: System.exit(1)
来源：http://ybz.ivvv.top

Go:   os.Exit(1)
来源：http://zzq.jinqigfzy.top

Ruby: exit 1
来源：http://vhz.fehbvm.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xhy.ivvv.top

[M06] 向标准错误输出
来源：http://lkv.ybcxt.top

Py:   print("err", file=sys.stderr)
来源：http://ibg.cdnleiting.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xib.xziqi.cn

JS:   console.error("err")
来源：http://esm.ywan-chungtsiang.top

TS:   console.error("err")
来源：http://aqe.nanxuanxn.top

Java: System.err.println("err")
来源：http://vzx.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://slg.jianghu66.top

Ruby: warn "err"
来源：http://rrr.yfazqb.com

C#:   Console.Error.WriteLine("err")
来源：http://zca.gzhubu.top

[M07] 判断是否为主入口
来源：http://pen.xuetiantiany.cn

Py:   if __name__ == "__main__":
来源：http://oyv.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ako.zhongyouzk.top

JS:   require.main === module
来源：http://xbj.xinyue.icu

TS:   require.main === module
来源：http://hub.tianlin.xyz

Java: public static void main(String[] args)
来源：http://okg.andypj.xyz

Go:   func main()
来源：http://qey.hongshengwenyu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hpm.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://pab.hcnkem.com

[M08] 获取系统与运行时信息
来源：http://hhr.xuanzx.com

Py:   platform.system();  platform.python_version()
来源：http://phj.wangshuangyany.cn

PHP:  PHP_OS;  phpversion();
来源：http://zyr.ybcxt.top

JS:   process.platform;  process.version
来源：http://all.ehwqpu.com

TS:   process.platform;  process.version
来源：http://edg.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://djt.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rmr.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lgq.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://glr.cheryme.top

================================================================================
来源：http://oht.hnxiangtu.top

N. 数据结构与算法
来源：http://ocv.xingfuxueyuan.xyz

================================================================================
来源：http://kew.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://rgw.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://viw.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ydw.ehwqpu.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oha.shzxlz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://syy.jianghu66.top

Java: Arrays.binarySearch(arr, x)
来源：http://epq.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://iyt.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://unr.gaohongyu789.top

C#:   Array.BinarySearch(arr, x)
来源：http://ygl.yonumen.top

[N02] 排序（工程实践用内置实现）
来源：http://awd.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://uyc.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gig.sxryk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xnu.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://ngb.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rvh.birdmap.top

Go:   slices.Sort(arr)
来源：http://kgf.quarkkingdee.top

Ruby: arr.sort
来源：http://cyg.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kwp.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://wuj.hfpthk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xiz.tarul.cn

PHP:  // 递归实现，或用 usort
来源：http://toq.fktsv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cnm.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://exw.nwbrower.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lzk.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zux.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yuh.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://oup.smart0.xyz

[N04] 斐波那契数列
来源：http://okz.aibaodan.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mhm.sjlbkw.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://org.hysaishi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jcu.chenjidiqi.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gkz.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vsr.hnxiangtu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://chy.sweek.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gnk.jinqigufen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wmk.yueranfly.top

[N05] 最大公约数
来源：http://nxk.wangshuangyany.cn

Py:   math.gcd(a, b)
来源：http://poy.daxiang520.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rvu.shanyushiyangtech.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pqy.hywenlv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dfz.jinqigfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vlx.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ycv.gzhubu.top

Ruby: a.gcd(b)
来源：http://dyu.kuanghao11.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://opk.haohaochexian.top

[N06] 判断回文字符串
来源：http://qge.jiagoushi.top

Py:   s == s[::-1]
来源：http://rvt.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://thy.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://lnj.zhiwuduotai.top

TS:   s === [...s].reverse().join("")
来源：http://lba.ywan-chungtsiang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://urc.epnwcf.com

Go:   // 双指针从两端比较
来源：http://gcq.fzhhl.top


<!-- 参考信息 -->