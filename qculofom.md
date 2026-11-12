代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rfv.yangfankeji.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tgd.hongshengwenyu.top

[J09] 时区处理
来源：http://iim.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rlo.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oka.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://svz.shangyingyoupin.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eqm.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mvx.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xcl.hnqzz.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vpz.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hbw.yj20258888.top

[J10] 取今天 / 本月第一天
来源：http://bry.zhiwuduotai.top

Py:   date.today();  date.today().replace(day=1)
来源：http://iyd.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rsx.ybcxt.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tfl.jlsjyb.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vyb.jqgfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dnt.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rnv.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ths.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xxq.yangfankeji.com

================================================================================
来源：http://fsh.hongshengwenyu.top

K. JSON 与序列化
来源：http://toq.shangyingyoupin.top

================================================================================
来源：http://iix.hcnkem.com

[K01] 对象转 JSON 字符串
来源：http://htj.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uyk.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dab.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://aqj.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://iwp.redwolf501.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yeo.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://xdo.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rak.sweek.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fli.yueranfly.top

[K02] JSON 字符串转对象
来源：http://xbz.zhiwuduotai.top

Py:   json.loads(s)
来源：http://fdf.svipenyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xyi.zycfv.cn

JS:   JSON.parse(s)
来源：http://aun.zhiwuduotai.top

TS:   JSON.parse(s)
来源：http://hqn.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dxt.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://lru.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://anz.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ypw.daxiang520.top

[K03] JSON 美化输出（带缩进）
来源：http://acn.wangdashe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xtw.zdqjudy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zot.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oiw.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wbn.svipenyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jqt.tarul.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lsc.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://kov.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rag.sweek.top

[K04] 读取 JSON 文件
来源：http://dok.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xtt.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rmi.yj20258.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jfv.ybcxt.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ssg.yj20258.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vwo.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iqx.cqqwz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qnj.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bzd.yueranfly.top

[K05] 深拷贝对象
来源：http://wqe.fengsongda.top

Py:   copy.deepcopy(obj)
来源：http://vdn.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://gws.nanxinkj.top

JS:   structuredClone(obj)
来源：http://eok.birdmap.top

TS:   structuredClone(obj)
来源：http://hoi.havefunace.top

Java: // 手写拷贝构造，或序列化往返
来源：http://soa.sysykeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nao.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://glg.shangyingyoupin.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jfn.yuxming.cn

[K06] 解析 URL 查询串
来源：http://dgm.hcnkem.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vzx.zdqjudy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://khw.ctjpmb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bkd.yuanzhike.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kad.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kwf.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lly.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wld.c1oappe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lgs.zhijiandao.cn

[K07] 进制转换
来源：http://zzw.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://flg.andypj.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://str.jinqigfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://grt.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xhw.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mjs.yj202588.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ayy.wangshuangyany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uel.gaohongyu789.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rpo.ywan-chungtsiang.top

[K08] 二进制序列化（非 JSON）
来源：http://wtv.ywan-chungtsiang.top

Py:   pickle.dumps(obj)
来源：http://phb.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://cdq.gogol.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://xlk.shanyushiyangtech.top

TS:   v8.serialize(obj)        // Node
来源：http://jea.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://coo.yj20258.top

Go:   encoding/gob
来源：http://dkq.yangfankeji.com

Ruby: Marshal.dump(obj)
来源：http://gao.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wbg.epnwcf.com

================================================================================
来源：http://cja.yanxiufei.cn

L. 网络请求
来源：http://tmb.zhengqikj.top

================================================================================
来源：http://dro.ctjpmb.com

[L01] 发送 GET 请求
来源：http://avq.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aas.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qtv.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://jgh.hywenlv.cn

TS:   await fetch(url)
来源：http://jhy.52xcode.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qiq.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://alb.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://bit.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://olr.smart0.xyz

[L02] 发送 POST JSON
来源：http://srm.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://egm.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ijb.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vit.cashguo.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aoe.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fho.yuxming.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gmx.xinyue.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ivv.fehbvm.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ndx.wangdashe.top

[L03] 设置自定义请求头
来源：http://goa.fzhhl.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nec.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://knl.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sec.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://osr.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qzh.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hzz.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aaq.jinqigfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ahm.chenjidiqi.icu

[L04] 设置超时
来源：http://uzg.sysykeji.top

Py:   requests.get(url, timeout=5)
来源：http://nmu.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ien.svipenyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kav.cashguo.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iee.xylfe.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gmp.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mon.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://unx.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xlz.daria6918.cn

[L05] 上传文件（multipart）
来源：http://rip.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ibj.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dqh.hcnkem.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yju.uphjek.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zrb.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tth.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://etl.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hrs.wangshuangyany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wxk.shangyingyoupin.top

[L06] 解析响应为 JSON
来源：http://fot.gotoacloud.top

Py:   resp.json()
来源：http://kwo.xziqi.cn

PHP:  json_decode($body, true);
来源：http://map.jinqigufen.top

JS:   await resp.json()
来源：http://cex.nwbrower.top

TS:   await resp.json()
来源：http://qey.ctjpmb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://txy.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cca.aizwys.cn

Ruby: JSON.parse(resp.body)
来源：http://pps.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yyj.zhiwuduotai.top

[L07] 处理 HTTP 状态码
来源：http://cfq.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gir.aizwys.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://svb.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://afa.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://ycw.yangfankeji.com

Java: resp.statusCode()
来源：http://kfm.yfazqb.com

Go:   resp.StatusCode
来源：http://ebw.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://rqo.hysaishi.cn

C#:   (int)resp.StatusCode
来源：http://aqi.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://kln.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://epy.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://vfm.nwbrower.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lvx.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hzy.hysaishi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oal.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gnp.feifeiyinyue.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bsr.ydzc1.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zcl.pycfn.com

================================================================================
来源：http://mpx.zdqjudy.top

M. 命令行 / 进程 / 环境
来源：http://tli.sxryk.cn

================================================================================
来源：http://wng.xinyue.icu

[M01] 读取命令行参数
来源：http://xse.9152youxi.cn

Py:   sys.argv[1:]
来源：http://gdr.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://gpr.epnwcf.com

JS:   process.argv.slice(2)
来源：http://ols.shanyushiyangkeji.top

TS:   process.argv.slice(2)
来源：http://fje.fengsongda.top

Java: args 数组（main 方法参数）
来源：http://ywt.hywenlv.cn

Go:   os.Args[1:]
来源：http://uer.xuetiantiany.cn

Ruby: ARGV
来源：http://spq.yuanzhike.top

C#:   args 数组（Main 方法参数）
来源：http://sry.hfpthk.cn

[M02] 读取环境变量
来源：http://cul.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://qtg.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bpo.ydjk.org.cn

JS:   process.env.HOME
来源：http://cnj.ppjwa.cn

TS:   process.env.HOME
来源：http://mzj.haohaochexian.top

Java: System.getenv("HOME")
来源：http://xws.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gah.tanke756.top

Ruby: ENV["HOME"]
来源：http://hht.nanxuanxn.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pua.chenzaomai.com

[M03] 执行外部命令
来源：http://awc.yueranfly.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mvo.jinqigfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hyt.yj202588.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ooe.ydzc1.top

TS:   child_process.execSync("ls -l").toString()
来源：http://buc.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dnz.andypj.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://onw.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://tds.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://pbw.fzhhl.top

[M04] 获取当前工作目录
来源：http://xsf.cashguo.top

Py:   os.getcwd()
来源：http://aav.yuanzhike.top

PHP:  getcwd();
来源：http://xox.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://ubq.nanxinkj.top

TS:   process.cwd()
来源：http://cmf.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://arc.gzhubu.top

Go:   os.Getwd()
来源：http://ndy.316326.xyz

Ruby: Dir.pwd
来源：http://nnn.shzxlz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vqn.svipenyu.cn

[M05] 设置退出码
来源：http://pvm.yueranfly.top

Py:   sys.exit(1)
来源：http://boi.gotoacloud.top

PHP:  exit(1);
来源：http://wnx.yueranfly.top

JS:   process.exit(1)
来源：http://wux.hcnkem.com

TS:   process.exit(1)
来源：http://qir.yfazqb.com

Java: System.exit(1)
来源：http://sxv.zhixingplan.top

Go:   os.Exit(1)
来源：http://fiv.haohaochexian.top

Ruby: exit 1
来源：http://gou.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hls.hysaishi.cn

[M06] 向标准错误输出
来源：http://erb.ydjk.org.cn

Py:   print("err", file=sys.stderr)
来源：http://ncd.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sya.yj202588.top

JS:   console.error("err")
来源：http://pst.zhaomingkeji.xyz

TS:   console.error("err")
来源：http://mur.uphjek.com

Java: System.err.println("err")
来源：http://cmc.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lqk.pengpengdd.cyou

Ruby: warn "err"
来源：http://kts.jinqigfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://cwl.havefunace.top

[M07] 判断是否为主入口
来源：http://cek.jqgfzy.top

Py:   if __name__ == "__main__":
来源：http://ewp.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://caa.cashguo.top

JS:   require.main === module
来源：http://nwe.nwbrower.top

TS:   require.main === module
来源：http://cur.ivvv.top

Java: public static void main(String[] args)
来源：http://oxv.fengsongda.top

Go:   func main()
来源：http://ibj.xingfuxueyuan.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qmq.yfazqb.com

C#:   static void Main(string[] args)
来源：http://xwd.jiagoushi.top

[M08] 获取系统与运行时信息
来源：http://mhh.tanke756.top

Py:   platform.system();  platform.python_version()
来源：http://nwu.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://kyk.zhoulong.xyz

JS:   process.platform;  process.version
来源：http://hia.shzxlz.cn

TS:   process.platform;  process.version
来源：http://cua.yangfankeji.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ora.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://lpp.zycfv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rjk.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://yad.epnwcf.com

================================================================================
来源：http://yzn.sjlbkw.cn

N. 数据结构与算法
来源：http://ukq.gogol.net.cn

================================================================================
来源：http://qsq.ivvv.top

[N01] 二分查找（有序数组）
来源：http://yar.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://bst.guowangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mof.ehwqpu.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lku.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vim.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://uhh.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://qus.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kla.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://hur.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://ilo.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://dvu.cdnleiting.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://btm.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pxd.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nud.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mbg.fzhhl.top

Go:   slices.Sort(arr)
来源：http://ohn.chenzaomai.com

Ruby: arr.sort
来源：http://ola.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jxj.jianghu66.top

[N03] 快速排序（分治示例）
来源：http://dod.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jwy.zhengqikj.top

PHP:  // 递归实现，或用 usort
来源：http://ylp.shuidangran.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ppw.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://scm.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oqp.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://raf.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zal.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://fzt.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://afq.ydjk.org.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vup.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://isg.yanxiufei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sls.yfazqb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zbz.chenjidiqi.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jwn.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cmo.yonumen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://daw.xuanzx.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bnz.hysaishi.cn

[N05] 最大公约数
来源：http://tla.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://jsh.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gyr.kuanghao11.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ssu.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wvj.jqgufenzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bjz.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zbt.52xcode.cn

Ruby: a.gcd(b)
来源：http://qeh.haohaochexian.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://twp.meibo888.top

[N06] 判断回文字符串
来源：http://srb.ydzc1.top

Py:   s == s[::-1]
来源：http://nrw.xuanzx.com

PHP:  $s === strrev($s);
来源：http://mtt.uphjek.com

JS:   s === [...s].reverse().join("")
来源：http://oxe.quarkkingdee.top

TS:   s === [...s].reverse().join("")
来源：http://nld.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qgh.havefunace.top

Go:   // 双指针从两端比较
来源：http://qrs.ivvv.top


<!-- 参考信息 -->