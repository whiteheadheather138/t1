代发 wailian999

Py:   (end - start).total_seconds()
来源：http://zkz.zhixingplan.top

PHP:  $end->diff($start)->days;
来源：http://ujg.chenzaomai.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://snb.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mep.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tue.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://vhk.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://put.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://yvs.mhx1999.top

[J07] 比较两个日期
来源：http://vkv.shanyushiyangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://zjq.xuetiantiany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://exz.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://rmq.snrcjt.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wjo.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mcl.bbcook.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lxw.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://bgv.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://fye.zhixingplan.top

[J08] 提取年月日与星期
来源：http://jer.jinyuanbaomall.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vex.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aof.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jdn.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tya.cucudq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://txm.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ees.yonumen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lsa.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wwt.uphjek.com

[J09] 时区处理
来源：http://gmw.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xxk.nanxuanxn.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fxj.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://seq.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hyc.hcnkem.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jxm.fanxiaobao.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gge.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bsm.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://enq.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://dpn.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ccz.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lsv.ehwqpu.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nog.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kyw.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wnd.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wld.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oph.52xcode.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kqz.shanyushiyangtech.top

================================================================================
来源：http://sfw.nanxinkj.top

K. JSON 与序列化
来源：http://pto.redwolf501.top

================================================================================
来源：http://lvv.pengpengdd.cyou

[K01] 对象转 JSON 字符串
来源：http://aus.redwolf501.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yuw.yuxming.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vtl.hesvh.cn

JS:   JSON.stringify(obj)
来源：http://sjb.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://dmh.wangshuangyany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vok.tianlin.xyz

Go:   json.Marshal(obj)
来源：http://myt.hysaishi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hsz.yj20258.top

C#:   JsonSerializer.Serialize(obj)
来源：http://awb.yangfankeji.com

[K02] JSON 字符串转对象
来源：http://xbp.jinqigufen.top

Py:   json.loads(s)
来源：http://daf.jlsjyb.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jbu.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://vkz.yonumen.top

TS:   JSON.parse(s)
来源：http://awq.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lrl.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://lfq.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://cvj.tarul.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ivl.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://lkp.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gnt.fengsongda.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rgr.c1oappe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://puq.ppjwa.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dkk.zhijiandao.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xda.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://syu.hesvh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mzi.ctjpmb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nfl.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://agf.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jel.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ljd.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oxn.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zjt.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://plu.bbcook.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mmm.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nmo.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pyu.bjfxy.top

[K05] 深拷贝对象
来源：http://hat.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://ngn.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://ddt.aibaodan.cn

JS:   structuredClone(obj)
来源：http://fmf.daria6918.cn

TS:   structuredClone(obj)
来源：http://yjc.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://jqx.shanyushiyangtech.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iej.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nic.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zxu.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://sfu.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://prx.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://myt.zhongyouzk.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://idj.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uqk.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mlx.9152youxi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://aoh.xziqi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uzp.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://stp.tian-w.cn

[K07] 进制转换
来源：http://agv.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tiv.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://clr.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wcc.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kcq.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wdo.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gpw.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gti.kuanghao11.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uiu.haohaochexian.top

[K08] 二进制序列化（非 JSON）
来源：http://xfj.aibaodan.cn

Py:   pickle.dumps(obj)
来源：http://zxb.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gyv.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://luf.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://tbj.vqdsnc.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jns.hnqzz.top

Go:   encoding/gob
来源：http://bwi.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://hpw.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://awj.dashuyun.cn

================================================================================
来源：http://cfx.chenzaomai.com

L. 网络请求
来源：http://zab.zdbjq.cn

================================================================================
来源：http://gzu.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://kub.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ymf.zdqjudy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://buq.havefunace.top

JS:   await fetch(url)
来源：http://iow.zhiwuduotai.top

TS:   await fetch(url)
来源：http://wql.sweek.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zvz.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://eus.shzxlz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bha.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fcj.shzxlz.cn

[L02] 发送 POST JSON
来源：http://bmi.vehdjk.com

Py:   requests.post(url, json={"a": 1})
来源：http://abp.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bup.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tqe.xuetiantiany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xmq.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://khc.xylfe.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cvy.aibaodan.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qpd.bjfxy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xlg.xziqi.cn

[L03] 设置自定义请求头
来源：http://ywr.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xym.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pqj.yuxming.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yoo.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pep.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://awl.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://urr.aibaodan.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bdz.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hza.snrcjt.cn

[L04] 设置超时
来源：http://kqx.yj20258888.top

Py:   requests.get(url, timeout=5)
来源：http://wql.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kub.c1oappe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yio.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pmd.pengpengdd.cyou

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zrq.zycfv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tdz.guannengcc.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bsw.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xhm.ybcxt.top

[L05] 上传文件（multipart）
来源：http://fjv.sufxvd.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pfq.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qmx.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zpx.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sbu.fehbvm.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ocm.c1oappe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lae.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jer.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kjk.iojbl.cn

[L06] 解析响应为 JSON
来源：http://mnt.yuxming.cn

Py:   resp.json()
来源：http://rmn.yfazqb.com

PHP:  json_decode($body, true);
来源：http://rmo.mhx1999.top

JS:   await resp.json()
来源：http://ptd.ydjk.org.cn

TS:   await resp.json()
来源：http://nus.yuxming.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://acd.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://buh.chenjidiqi.icu

Ruby: JSON.parse(resp.body)
来源：http://ass.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://odk.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://nxk.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hzp.tian-w.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://npu.ppjwa.cn

JS:   resp.ok;  resp.status
来源：http://lqj.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://ztt.iojbl.cn

Java: resp.statusCode()
来源：http://cqu.mhx1999.top

Go:   resp.StatusCode
来源：http://bfd.svipenyu.cn

Ruby: resp.code.to_i
来源：http://rfm.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://pam.cqqwz.cn

[L08] 并发请求多个地址
来源：http://txy.xziqi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nbq.redwolf501.top

PHP:  curl_multi_init() 系列
来源：http://gqr.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mbm.nanxinkj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gtf.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lrg.zhijiandao.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qtc.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bqw.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sgc.jqgfzy.top

================================================================================
来源：http://pez.tianlin.xyz

M. 命令行 / 进程 / 环境
来源：http://rzm.c1oappe.top

================================================================================
来源：http://pvk.zhengqikj.top

[M01] 读取命令行参数
来源：http://oah.9152youxi.cn

Py:   sys.argv[1:]
来源：http://szw.sweek.top

PHP:  $argv;  $argc;
来源：http://upn.iojbl.cn

JS:   process.argv.slice(2)
来源：http://jse.fktsv.cn

TS:   process.argv.slice(2)
来源：http://unx.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://qgg.xuanzx.com

Go:   os.Args[1:]
来源：http://zvu.feifeiyinyue.top

Ruby: ARGV
来源：http://ygj.ydzc1.top

C#:   args 数组（Main 方法参数）
来源：http://qkq.nanxuanxn.top

[M02] 读取环境变量
来源：http://kgy.sysykeji.top

Py:   os.environ.get("HOME")
来源：http://wwb.ppjwa.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rwf.bjfxy.top

JS:   process.env.HOME
来源：http://xza.jianghu66.top

TS:   process.env.HOME
来源：http://qqx.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://kce.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hhs.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://uad.zhoulong.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rcn.ctjpmb.com

[M03] 执行外部命令
来源：http://lag.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sfq.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ugr.chenlongwang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://frh.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rvn.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zww.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nbj.zdbjq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qbk.tian-w.cn

C#:   Process.Start("ls", "-l");
来源：http://pkn.fengsongda.top

[M04] 获取当前工作目录
来源：http://gad.vehdjk.com

Py:   os.getcwd()
来源：http://nwe.chenlongwang.top

PHP:  getcwd();
来源：http://ndd.yongpay.top

JS:   process.cwd()
来源：http://ykh.xylfe.cn

TS:   process.cwd()
来源：http://rdc.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://ftp.hysaishi.cn

Go:   os.Getwd()
来源：http://lfx.c1oappe.top

Ruby: Dir.pwd
来源：http://bde.yongpay.top

C#:   Directory.GetCurrentDirectory()
来源：http://tow.andypj.xyz

[M05] 设置退出码
来源：http://mwk.shanyushiyangtech.top

Py:   sys.exit(1)
来源：http://xtu.pycfn.com

PHP:  exit(1);
来源：http://hho.sjlbkw.cn

JS:   process.exit(1)
来源：http://dyx.52xcode.cn

TS:   process.exit(1)
来源：http://voj.tanke756.top

Java: System.exit(1)
来源：http://duw.cucudq.cn

Go:   os.Exit(1)
来源：http://bfy.yanxiufei.cn

Ruby: exit 1
来源：http://trd.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://spi.zhixingplan.top

[M06] 向标准错误输出
来源：http://wph.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://yef.quarkkingdee.top

PHP:  fwrite(STDERR, "err\n");
来源：http://reo.yanxiufei.cn

JS:   console.error("err")
来源：http://off.hywenlv.cn

TS:   console.error("err")
来源：http://nrg.shzxlz.cn

Java: System.err.println("err")
来源：http://afd.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wlm.haohaochexian.top

Ruby: warn "err"
来源：http://iuk.zhengqikj.top

C#:   Console.Error.WriteLine("err")
来源：http://poz.havefunace.top

[M07] 判断是否为主入口
来源：http://sow.guannengcc.top

Py:   if __name__ == "__main__":
来源：http://gdk.gogol.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kui.jinqigfzy.top

JS:   require.main === module
来源：http://aen.chenzaomai.com

TS:   require.main === module
来源：http://zsd.daria6918.cn

Java: public static void main(String[] args)
来源：http://ujk.guannengcc.top

Go:   func main()
来源：http://dfl.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://veo.kuanghao11.cn

C#:   static void Main(string[] args)
来源：http://beb.sjlbkw.cn

[M08] 获取系统与运行时信息
来源：http://sme.yfazqb.com

Py:   platform.system();  platform.python_version()
来源：http://lac.sweek.top

PHP:  PHP_OS;  phpversion();
来源：http://vzm.ppjwa.cn

JS:   process.platform;  process.version
来源：http://tzv.nanxuanxn.top

TS:   process.platform;  process.version
来源：http://cze.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gvl.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://kco.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pdx.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kvo.xuetiantiany.cn

================================================================================
来源：http://usp.vqdsnc.cn

N. 数据结构与算法
来源：http://sir.ppjwa.cn

================================================================================
来源：http://zzv.316326.xyz

[N01] 二分查找（有序数组）
来源：http://pbm.tian-w.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cwt.wangdashe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jhv.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hom.yj20258888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ezd.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yab.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://vdj.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://poc.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gpd.uphjek.com

[N02] 排序（工程实践用内置实现）
来源：http://din.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://koh.zhixingplan.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gfg.bbcook.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uqf.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nym.zhaomingkeji.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gbs.cheryme.top

Go:   slices.Sort(arr)
来源：http://jqr.jlsjyb.cn

Ruby: arr.sort
来源：http://lma.meibo888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xts.svipenyu.cn

[N03] 快速排序（分治示例）
来源：http://pec.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gis.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://wtw.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bjk.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://plj.ehwqpu.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lrx.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ywd.hfpthk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zoh.jiagoushi.top

C#:   // 手写递归，或 Array.Sort
来源：http://vnd.316326.xyz

[N04] 斐波那契数列
来源：http://nfu.daxiang520.top


<!-- 参考信息 -->