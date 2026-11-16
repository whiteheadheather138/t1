代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://enu.yvedp.cn

[J08] 提取年月日与星期
来源：http://ryj.daria6918.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wgm.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sgi.shzxlz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mqn.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://auw.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mqz.ppjwa.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://orj.hammf.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://drv.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ldv.ybcxt.top

[J09] 时区处理
来源：http://xky.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tgn.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oae.jinqigfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tey.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ygk.gaohongyu789.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rpj.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://utp.feifeiyinyue.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lsu.xuanzx.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zuy.xinyue.icu

[J10] 取今天 / 本月第一天
来源：http://ydx.yangfankeji.com

Py:   date.today();  date.today().replace(day=1)
来源：http://hdu.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hah.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://puh.xingfuxueyuan.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ybv.aibaodan.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ffn.birdmap.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yoa.chenjidiqi.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://grx.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cuu.cqqwz.cn

================================================================================
来源：http://vmc.sxryk.cn

K. JSON 与序列化
来源：http://cna.yongpay.top

================================================================================
来源：http://mpt.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://ptc.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lwj.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lqy.havefunace.top

JS:   JSON.stringify(obj)
来源：http://axs.fanxiaobao.xyz

TS:   JSON.stringify(obj)
来源：http://bud.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fib.daria6918.cn

Go:   json.Marshal(obj)
来源：http://rou.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://tkb.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fij.jiagoushi.top

[K02] JSON 字符串转对象
来源：http://ifi.jinghuilouyu.cn

Py:   json.loads(s)
来源：http://hbp.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fyk.xylfe.cn

JS:   JSON.parse(s)
来源：http://xvz.quarkkingdee.top

TS:   JSON.parse(s)
来源：http://uea.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fan.gzhubu.top

Go:   json.Unmarshal(data, &v)
来源：http://ukd.fzhhl.top

Ruby: JSON.parse(s)
来源：http://ghi.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://frz.guowangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://hfs.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://klo.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ieh.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jcl.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vud.hnxiangtu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fls.cheryme.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://leg.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://yoq.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://srf.jlsjyb.cn

[K04] 读取 JSON 文件
来源：http://wob.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://poc.xingfuxueyuan.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xhn.nanxuanxn.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zkh.jlsjyb.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://job.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hcb.yj20258888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fos.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xvd.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ooa.yj20258.top

[K05] 深拷贝对象
来源：http://rcy.jianghu66.top

Py:   copy.deepcopy(obj)
来源：http://eqr.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://sfa.jqgfzy.top

JS:   structuredClone(obj)
来源：http://zir.redwolf501.top

TS:   structuredClone(obj)
来源：http://nqt.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xem.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nwy.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ojw.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ybv.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://lgy.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rve.ehwqpu.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://esr.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://okw.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nsv.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fhy.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://llt.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kku.316326.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://doj.shanyushiyangkeji.top

[K07] 进制转换
来源：http://ktr.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dca.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://whd.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fyd.mhx1999.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://imy.nanxinkj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jdk.shanyushiyangtech.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lvt.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qih.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://myl.shanyushiyangtech.top

[K08] 二进制序列化（非 JSON）
来源：http://xsd.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://eri.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gsz.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://tny.daxiang520.top

TS:   v8.serialize(obj)        // Node
来源：http://gkj.shuidangran.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jkk.52xcode.cn

Go:   encoding/gob
来源：http://uvp.sweek.top

Ruby: Marshal.dump(obj)
来源：http://pwn.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xsn.zdbjq.cn

================================================================================
来源：http://fao.zhoulong.xyz

L. 网络请求
来源：http://jux.smart0.xyz

================================================================================
来源：http://jrh.cashguo.top

[L01] 发送 GET 请求
来源：http://ymf.jianghu66.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vpd.jiagoushi.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xgk.dianchejie.cn

JS:   await fetch(url)
来源：http://crr.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://rpf.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zou.zhongyouzk.top

Go:   resp, err := http.Get(url)
来源：http://frz.hesvh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eth.guowangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qrf.yonumen.top

[L02] 发送 POST JSON
来源：http://mwo.hammf.cn

Py:   requests.post(url, json={"a": 1})
来源：http://aws.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lsr.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://psg.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ldi.ivvv.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zyc.fanxiaobao.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ayf.havefunace.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://brv.chenjidiqi.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qma.jinghuilouyu.cn

[L03] 设置自定义请求头
来源：http://zeb.zhaomingkeji.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vjo.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iph.c1oappe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uot.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ebo.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xsn.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wfx.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://swf.sufxvd.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rit.ivvv.top

[L04] 设置超时
来源：http://nxa.cucudq.cn

Py:   requests.get(url, timeout=5)
来源：http://vgr.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uzh.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://egl.ydjk.org.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xxr.jyoumei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rqw.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cqc.hongshengwenyu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mua.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nwh.zhongyouzk.top

[L05] 上传文件（multipart）
来源：http://jdr.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vow.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jtf.sjlbkw.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ect.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eep.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kbj.hammf.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jek.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vxs.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tvg.andypj.xyz

[L06] 解析响应为 JSON
来源：http://gbb.sysykeji.top

Py:   resp.json()
来源：http://kxv.quarkkingdee.top

PHP:  json_decode($body, true);
来源：http://dnw.hywenlv.cn

JS:   await resp.json()
来源：http://baa.gaohongyu789.top

TS:   await resp.json()
来源：http://gqy.zhijiandao.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lpv.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mnd.ydjk.org.cn

Ruby: JSON.parse(resp.body)
来源：http://abg.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yxd.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://qmw.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fhm.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jik.316326.xyz

JS:   resp.ok;  resp.status
来源：http://emi.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://ohp.shzxlz.cn

Java: resp.statusCode()
来源：http://pva.cheryme.top

Go:   resp.StatusCode
来源：http://knw.yj20258.top

Ruby: resp.code.to_i
来源：http://uri.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://nvb.ybcxt.top

[L08] 并发请求多个地址
来源：http://rij.sjlbkw.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ppl.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://obm.aizwys.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jzu.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ebt.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jyq.ppjwa.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oeo.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://den.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ggz.yj20258888.top

================================================================================
来源：http://eey.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://upf.yonumen.top

================================================================================
来源：http://ado.zycfv.cn

[M01] 读取命令行参数
来源：http://uvs.zhijiandao.cn

Py:   sys.argv[1:]
来源：http://quc.c1oappe.top

PHP:  $argv;  $argc;
来源：http://que.yvedp.cn

JS:   process.argv.slice(2)
来源：http://fsn.xinyue.icu

TS:   process.argv.slice(2)
来源：http://des.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://mpp.guowangkeji.top

Go:   os.Args[1:]
来源：http://vnu.tian-w.cn

Ruby: ARGV
来源：http://jgv.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://hmk.yuanzhike.top

[M02] 读取环境变量
来源：http://xhw.zhiwuduotai.top

Py:   os.environ.get("HOME")
来源：http://bfn.xuanzx.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sai.xuanzx.com

JS:   process.env.HOME
来源：http://ohd.tarul.cn

TS:   process.env.HOME
来源：http://tve.birdmap.top

Java: System.getenv("HOME")
来源：http://oji.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vxo.fzhhl.top

Ruby: ENV["HOME"]
来源：http://xal.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lca.c1oappe.top

[M03] 执行外部命令
来源：http://rll.bbcook.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kgm.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mbf.fktsv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zxy.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://bdg.zhaomingkeji.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ozx.jinyuanbaomall.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hos.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://lmy.tian-w.cn

C#:   Process.Start("ls", "-l");
来源：http://gpk.jqgfzy.top

[M04] 获取当前工作目录
来源：http://qhz.zhixingplan.top

Py:   os.getcwd()
来源：http://hvn.hesvh.cn

PHP:  getcwd();
来源：http://xmy.c1oappe.top

JS:   process.cwd()
来源：http://zcy.hesvh.cn

TS:   process.cwd()
来源：http://mcp.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://drm.ivvv.top

Go:   os.Getwd()
来源：http://wrs.yongpay.top

Ruby: Dir.pwd
来源：http://ntu.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vwg.jqgfzy.top

[M05] 设置退出码
来源：http://xea.yj202588.top

Py:   sys.exit(1)
来源：http://xuf.jqgfzy.top

PHP:  exit(1);
来源：http://hyg.jlsjyb.cn

JS:   process.exit(1)
来源：http://krz.tian-w.cn

TS:   process.exit(1)
来源：http://jdt.yangfankeji.com

Java: System.exit(1)
来源：http://huz.xingfuxueyuan.xyz

Go:   os.Exit(1)
来源：http://jir.mhx1999.top

Ruby: exit 1
来源：http://axd.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wya.hfpthk.cn

[M06] 向标准错误输出
来源：http://mss.yuanzhike.top

Py:   print("err", file=sys.stderr)
来源：http://nqv.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fau.yangfankeji.com

JS:   console.error("err")
来源：http://bef.fzhhl.top

TS:   console.error("err")
来源：http://zll.andypj.xyz

Java: System.err.println("err")
来源：http://yhd.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mhm.redwolf501.top

Ruby: warn "err"
来源：http://evc.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://kla.jqgufenzy.top

[M07] 判断是否为主入口
来源：http://dll.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://etr.smart0.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iud.birdmap.top

JS:   require.main === module
来源：http://pjk.shanyushiyangkeji.top

TS:   require.main === module
来源：http://zzy.smart0.xyz

Java: public static void main(String[] args)
来源：http://ohr.gaohongyu789.top

Go:   func main()
来源：http://ebe.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gru.zycfv.cn

C#:   static void Main(string[] args)
来源：http://arl.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://wje.snrcjt.cn

Py:   platform.system();  platform.python_version()
来源：http://ifs.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://weu.ehwqpu.com

JS:   process.platform;  process.version
来源：http://xky.jiagoushi.top

TS:   process.platform;  process.version
来源：http://dym.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bny.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://hno.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zzy.aibaodan.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dkg.ydzc1.top

================================================================================
来源：http://edk.feifeiyinyue.top

N. 数据结构与算法
来源：http://fqk.xinyue.icu

================================================================================
来源：http://hyn.pycfn.com

[N01] 二分查找（有序数组）
来源：http://ezq.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ndu.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://azh.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zyx.sjlbkw.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tvp.nwbrower.top

Java: Arrays.binarySearch(arr, x)
来源：http://drk.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://vnw.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://voi.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://flf.yfazqb.com

[N02] 排序（工程实践用内置实现）
来源：http://ufy.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://nua.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yab.xuanzx.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ggx.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://chf.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ibo.aizwys.cn

Go:   slices.Sort(arr)
来源：http://cwq.shanyushiyangtech.top

Ruby: arr.sort
来源：http://cya.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tsn.gogol.net.cn

[N03] 快速排序（分治示例）
来源：http://lut.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cbm.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://app.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wyq.yj20258.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ixn.tianlin.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oqd.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dmq.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://obw.tian-w.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lwm.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://msw.redwolf501.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vzi.ydzc1.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://myg.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tcc.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hnb.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mcs.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ils.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://liz.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gzi.cdnleiting.top

[N05] 最大公约数
来源：http://msh.yonumen.top

Py:   math.gcd(a, b)
来源：http://oyp.nanxinkj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bfc.yongpay.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iak.wangshuangyany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jot.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xcz.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://scw.shanyushiyangkeji.top

Ruby: a.gcd(b)
来源：http://hlm.ydjk.org.cn


<!-- 参考信息 -->