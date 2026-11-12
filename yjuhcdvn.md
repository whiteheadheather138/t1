代发 wailian999

[J07] 比较两个日期
来源：http://nrn.sufxvd.cn

Py:   d1 < d2;  d1 == d2
来源：http://jzi.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mrs.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://mqu.hnxiangtu.top

TS:   d1.getTime() < d2.getTime()
来源：http://nld.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://who.cdnleiting.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kfs.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://roz.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://sni.yj202588.top

[J08] 提取年月日与星期
来源：http://vqq.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eva.chenlongwang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wzq.jqgufenzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aen.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lgy.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xya.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lla.hammf.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sxf.xziqi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eex.wangdashe.top

[J09] 时区处理
来源：http://sao.hongshengwenyu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qfx.zhiwuduotai.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cpi.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kan.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ayc.wangshuangyany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zjx.hnxiangtu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://anc.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eck.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://std.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://jca.gaohongyu789.top

Py:   date.today();  date.today().replace(day=1)
来源：http://piy.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fql.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://otd.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ctm.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vbx.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://voz.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ehl.xylfe.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xhr.daxiang520.top

================================================================================
来源：http://emq.cashguo.top

K. JSON 与序列化
来源：http://qwl.nanxuanxn.top

================================================================================
来源：http://qas.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://pcn.zhoulong.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://njm.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cei.ivvv.top

JS:   JSON.stringify(obj)
来源：http://nub.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://zxj.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://guj.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://iea.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://ssl.ivvv.top

C#:   JsonSerializer.Serialize(obj)
来源：http://thi.fktsv.cn

[K02] JSON 字符串转对象
来源：http://yrt.shanyushiyangtech.top

Py:   json.loads(s)
来源：http://nmr.gotoacloud.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pao.zhengqikj.top

JS:   JSON.parse(s)
来源：http://ves.fanxiaobao.xyz

TS:   JSON.parse(s)
来源：http://ono.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mps.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://nng.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://eoh.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bjw.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://yfg.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hnc.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lat.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cfv.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://rdw.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fdi.cheryme.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ztg.316326.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://pjq.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eba.nwbrower.top

[K04] 读取 JSON 文件
来源：http://efh.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rxr.zycfv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://drw.nanxuanxn.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yti.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wxe.ppjwa.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lbn.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aeb.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pag.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hmq.jqgfzy.top

[K05] 深拷贝对象
来源：http://nto.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://qdk.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://iyt.dashuyun.cn

JS:   structuredClone(obj)
来源：http://mkt.pengpengdd.cyou

TS:   structuredClone(obj)
来源：http://zft.cdnleiting.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tiq.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rjq.jinghuilouyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yae.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://tkd.shuidangran.top

[K06] 解析 URL 查询串
来源：http://wjp.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rxb.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qno.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cyr.ppjwa.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iyw.cdnleiting.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hfv.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oqz.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fjh.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jlk.cucudq.cn

[K07] 进制转换
来源：http://bvn.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qpm.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tyq.svipenyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rsj.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://msh.ywan-chungtsiang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lid.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://twp.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dez.xziqi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hbc.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://vpj.tanke756.top

Py:   pickle.dumps(obj)
来源：http://vjm.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wrr.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://amu.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://kwt.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cth.guannengcc.top

Go:   encoding/gob
来源：http://tlw.yongpay.top

Ruby: Marshal.dump(obj)
来源：http://plz.yj202588.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ebu.zdqjudy.top

================================================================================
来源：http://xhy.yonumen.top

L. 网络请求
来源：http://pot.gzhubu.top

================================================================================
来源：http://prj.c1oappe.top

[L01] 发送 GET 请求
来源：http://zib.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yhp.0kj1m.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ikw.mhx1999.top

JS:   await fetch(url)
来源：http://pvu.tianlin.xyz

TS:   await fetch(url)
来源：http://vzr.epnwcf.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wco.hysaishi.cn

Go:   resp, err := http.Get(url)
来源：http://yuf.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bhr.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gpn.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://sym.hnqzz.top

Py:   requests.post(url, json={"a": 1})
来源：http://zqd.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dlm.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mmk.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zqw.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lzb.yanxiufei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eod.yfazqb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vqp.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fik.zhongyouzk.top

[L03] 设置自定义请求头
来源：http://guc.hywenlv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ugy.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dbu.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cgf.xingfuxueyuan.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://evq.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://njp.52xcode.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wfh.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gee.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oln.chenjidiqi.icu

[L04] 设置超时
来源：http://jwk.xuetiantiany.cn

Py:   requests.get(url, timeout=5)
来源：http://bao.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dsv.jiagoushi.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cgi.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yhi.jqgfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fqf.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dwo.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xuf.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vqe.jianghu66.top

[L05] 上传文件（multipart）
来源：http://xvi.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wlx.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gxg.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tgs.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://krp.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jbq.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mrr.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jqt.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oco.vehdjk.com

[L06] 解析响应为 JSON
来源：http://zvz.iojbl.cn

Py:   resp.json()
来源：http://fpt.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://ecx.jqgfzy.top

JS:   await resp.json()
来源：http://etr.jlsjyb.cn

TS:   await resp.json()
来源：http://lap.shanyushiyangtech.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bek.hongshengwenyu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gqi.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://rkj.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://guj.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://tdo.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yrf.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fcq.yvedp.cn

JS:   resp.ok;  resp.status
来源：http://uvw.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://eog.nanxinkj.top

Java: resp.statusCode()
来源：http://hdt.fzhhl.top

Go:   resp.StatusCode
来源：http://iie.daxiang520.top

Ruby: resp.code.to_i
来源：http://mhc.hysaishi.cn

C#:   (int)resp.StatusCode
来源：http://xem.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://wyz.ywan-chungtsiang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tey.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://bnl.hnqzz.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kpp.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rko.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ntz.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ptg.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jqq.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bct.jyoumei.cn

================================================================================
来源：http://zmm.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://awk.fanxiaobao.xyz

================================================================================
来源：http://gao.fehbvm.com

[M01] 读取命令行参数
来源：http://zts.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://nqk.nanxinkj.top

PHP:  $argv;  $argc;
来源：http://udn.mhx1999.top

JS:   process.argv.slice(2)
来源：http://gwt.meibo888.top

TS:   process.argv.slice(2)
来源：http://dni.fehbvm.com

Java: args 数组（main 方法参数）
来源：http://tzk.tarul.cn

Go:   os.Args[1:]
来源：http://czl.xuetiantiany.cn

Ruby: ARGV
来源：http://uuk.ywan-chungtsiang.top

C#:   args 数组（Main 方法参数）
来源：http://akb.hnqzz.top

[M02] 读取环境变量
来源：http://ccq.chenjidiqi.icu

Py:   os.environ.get("HOME")
来源：http://gft.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vmo.yfazqb.com

JS:   process.env.HOME
来源：http://hco.pengpengdd.cyou

TS:   process.env.HOME
来源：http://fub.wangdashe.top

Java: System.getenv("HOME")
来源：http://kaq.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fim.andypj.xyz

Ruby: ENV["HOME"]
来源：http://ilb.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hvs.zycfv.cn

[M03] 执行外部命令
来源：http://yzn.sysykeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://unr.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xmi.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uxu.ydjk.org.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pcu.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pwm.cheryme.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gsw.cdnleiting.top

Ruby: system("ls -l");  `ls -l`
来源：http://tji.feifeiyinyue.top

C#:   Process.Start("ls", "-l");
来源：http://ghm.fanxiaobao.xyz

[M04] 获取当前工作目录
来源：http://jit.jianghu66.top

Py:   os.getcwd()
来源：http://fkt.cheryme.top

PHP:  getcwd();
来源：http://vvu.ppjwa.cn

JS:   process.cwd()
来源：http://jwi.jlsjyb.cn

TS:   process.cwd()
来源：http://fdb.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://hdy.ydjk.org.cn

Go:   os.Getwd()
来源：http://awd.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://viu.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://pno.yj202588.top

[M05] 设置退出码
来源：http://imq.nanxinkj.top

Py:   sys.exit(1)
来源：http://gvg.xziqi.cn

PHP:  exit(1);
来源：http://fld.daxiang520.top

JS:   process.exit(1)
来源：http://hxs.hywenlv.cn

TS:   process.exit(1)
来源：http://uxb.smart0.xyz

Java: System.exit(1)
来源：http://rmy.jinqigfzy.top

Go:   os.Exit(1)
来源：http://ejr.chenlongwang.top

Ruby: exit 1
来源：http://fhp.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ykp.jyoumei.cn

[M06] 向标准错误输出
来源：http://prw.tian-w.cn

Py:   print("err", file=sys.stderr)
来源：http://wni.c1oappe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qld.vehdjk.com

JS:   console.error("err")
来源：http://dic.hesvh.cn

TS:   console.error("err")
来源：http://dsw.daxiang520.top

Java: System.err.println("err")
来源：http://orl.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oah.52xcode.cn

Ruby: warn "err"
来源：http://xqc.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://aod.0kj1m.cn

[M07] 判断是否为主入口
来源：http://nzm.hcnkem.com

Py:   if __name__ == "__main__":
来源：http://bje.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sba.pycfn.com

JS:   require.main === module
来源：http://szk.pycfn.com

TS:   require.main === module
来源：http://lpl.jyoumei.cn

Java: public static void main(String[] args)
来源：http://obj.ehwqpu.com

Go:   func main()
来源：http://izg.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oxc.xziqi.cn

C#:   static void Main(string[] args)
来源：http://biv.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://qwi.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://vcv.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://oim.guannengcc.top

JS:   process.platform;  process.version
来源：http://tiy.tanke756.top

TS:   process.platform;  process.version
来源：http://zij.hnxiangtu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rvl.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qoa.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qed.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dsj.uphjek.com

================================================================================
来源：http://bzl.yonumen.top

N. 数据结构与算法
来源：http://soc.shzxlz.cn

================================================================================
来源：http://rmq.uphjek.com

[N01] 二分查找（有序数组）
来源：http://ujj.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://lfa.cucudq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cyo.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sfn.jyoumei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://csl.0kj1m.cn

Java: Arrays.binarySearch(arr, x)
来源：http://car.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://axm.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://yfh.yfazqb.com

C#:   Array.BinarySearch(arr, x)
来源：http://ves.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://tuj.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://rnh.snrcjt.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ytf.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tam.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lje.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://npx.chenzaomai.com

Go:   slices.Sort(arr)
来源：http://oee.snrcjt.cn

Ruby: arr.sort
来源：http://oyn.xylfe.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rbk.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://lpk.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hwb.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://ati.hywenlv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nwf.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ufw.jiagoushi.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eoq.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vrn.snrcjt.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pqn.snrcjt.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ahn.yj20258.top

[N04] 斐波那契数列
来源：http://dvx.zhiwuduotai.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wls.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bfc.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kjk.yangfankeji.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kdl.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lzs.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dyk.yj20258.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yjt.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eqt.nwbrower.top


<!-- 参考信息 -->