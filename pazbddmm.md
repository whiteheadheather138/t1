代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://bzo.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eas.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://euy.zhaomingkeji.xyz

Java: LocalDate.now().plusDays(7)
来源：http://jcb.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zvq.316326.xyz

Ruby: Time.now + 7 * 86400
来源：http://iwx.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://wsh.shuidangran.top

[J06] 计算两时间之差
来源：http://may.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://rbc.ctjpmb.com

PHP:  $end->diff($start)->days;
来源：http://wqv.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://brs.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nkh.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://jro.jinyuanbaomall.cn

Go:   end.Sub(start).Hours()
来源：http://ovd.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://igs.ctjpmb.com

C#:   (end - start).TotalSeconds
来源：http://zeb.svipenyu.cn

[J07] 比较两个日期
来源：http://vrv.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://mwa.fzhhl.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rsi.jiagoushi.top

JS:   d1.getTime() < d2.getTime()
来源：http://dne.jlsjyb.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dpc.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yon.jyoumei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cwx.yfazqb.com

Ruby: d1 < d2;  d1 == d2
来源：http://lwr.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://xbe.bbcook.cn

[J08] 提取年月日与星期
来源：http://ccw.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vfg.ctjpmb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hjo.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lcp.xziqi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://msf.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zig.smart0.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jhb.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sbd.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jpj.9152youxi.cn

[J09] 时区处理
来源：http://klv.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gkv.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yay.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wwq.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iyt.nwbrower.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ccr.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bls.hnqzz.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jxx.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://crq.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://rsu.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cis.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tgj.shzxlz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aom.jinqigfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ikr.yuxming.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mja.sweek.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zib.ehwqpu.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ubz.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://abp.feifeiyinyue.top

================================================================================
来源：http://lrj.yueranfly.top

K. JSON 与序列化
来源：http://hak.hongshengwenyu.top

================================================================================
来源：http://jio.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://cdw.pengpengdd.cyou

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://obm.redwolf501.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pzu.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://rvy.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://tsd.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mom.bbcook.cn

Go:   json.Marshal(obj)
来源：http://llo.ctjpmb.com

Ruby: obj.to_json                                     // require "json"
来源：http://bky.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://tem.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://tcc.yj20258888.top

Py:   json.loads(s)
来源：http://gnx.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mcb.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://juj.svipenyu.cn

TS:   JSON.parse(s)
来源：http://spo.feifeiyinyue.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xmf.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://mfa.vehdjk.com

Ruby: JSON.parse(s)
来源：http://wfn.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cap.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://lxt.gaohongyu789.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ubh.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tjk.jqgufenzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wgg.xinyue.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://ari.yueranfly.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://klc.tarul.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://duw.havefunace.top

Ruby: JSON.pretty_generate(obj)
来源：http://wtg.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kad.yj202588.top

[K04] 读取 JSON 文件
来源：http://haf.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qyr.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rvj.sysykeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yxk.ydjk.org.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hbk.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xvw.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tpt.sufxvd.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://loq.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wfp.ybcxt.top

[K05] 深拷贝对象
来源：http://zmv.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://yjo.redwolf501.top

PHP:  unserialize(serialize($obj));
来源：http://hyb.fengsongda.top

JS:   structuredClone(obj)
来源：http://fcs.ivvv.top

TS:   structuredClone(obj)
来源：http://bqx.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cop.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iuf.wangshuangyany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cxn.shanyushiyangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ved.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://ycn.yanxiufei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://udx.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yzi.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://otc.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iyg.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://slc.ydjk.org.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://asg.hnxiangtu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bkq.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dbc.zdbjq.cn

[K07] 进制转换
来源：http://jbo.guannengcc.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pnq.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dur.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uxg.feifeiyinyue.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zem.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zfr.xuetiantiany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pgq.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://awz.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://whb.daxiang520.top

[K08] 二进制序列化（非 JSON）
来源：http://iwu.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://ttl.zdbjq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nug.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://rcm.fehbvm.com

TS:   v8.serialize(obj)        // Node
来源：http://opy.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hds.cucudq.cn

Go:   encoding/gob
来源：http://ukb.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://iye.vqdsnc.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yaz.yuxming.cn

================================================================================
来源：http://exm.xingfuxueyuan.xyz

L. 网络请求
来源：http://moe.ppjwa.cn

================================================================================
来源：http://ugs.hywenlv.cn

[L01] 发送 GET 请求
来源：http://vye.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jct.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ywa.hongshengwenyu.top

JS:   await fetch(url)
来源：http://bpv.tianlin.xyz

TS:   await fetch(url)
来源：http://smp.yongpay.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://prx.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://tya.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://iky.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yrd.chenzaomai.com

[L02] 发送 POST JSON
来源：http://vgp.pycfn.com

Py:   requests.post(url, json={"a": 1})
来源：http://exk.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://etq.kuanghao11.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://etv.hywenlv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ghw.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eli.shanyushiyangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aby.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sav.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pks.gotoacloud.top

[L03] 设置自定义请求头
来源：http://qul.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jxz.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ptr.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rad.0kj1m.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hid.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hlw.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qwk.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://acj.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gpz.nanxuanxn.top

[L04] 设置超时
来源：http://mht.haohaochexian.top

Py:   requests.get(url, timeout=5)
来源：http://lhw.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wlx.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ovm.guannengcc.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cse.jyoumei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gbc.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gcc.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://phf.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kyk.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://rhg.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://swz.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rri.jqgfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rnl.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pks.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ztk.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mbk.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ggz.yuanzhike.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xwc.yuxming.cn

[L06] 解析响应为 JSON
来源：http://ixq.zhengqikj.top

Py:   resp.json()
来源：http://kmh.ydjk.org.cn

PHP:  json_decode($body, true);
来源：http://iov.shanyushiyangtech.top

JS:   await resp.json()
来源：http://xjc.chenzaomai.com

TS:   await resp.json()
来源：http://ujp.yonumen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ela.zhijiandao.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xee.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://uyv.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://urt.tanke756.top

[L07] 处理 HTTP 状态码
来源：http://xjc.jinqigfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vvn.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://msf.daria6918.cn

JS:   resp.ok;  resp.status
来源：http://kvv.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://hvc.feifeiyinyue.top

Java: resp.statusCode()
来源：http://sqn.52xcode.cn

Go:   resp.StatusCode
来源：http://gyz.jinqigfzy.top

Ruby: resp.code.to_i
来源：http://kaa.ybcxt.top

C#:   (int)resp.StatusCode
来源：http://trz.cqqwz.cn

[L08] 并发请求多个地址
来源：http://frm.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cih.chenjidiqi.icu

PHP:  curl_multi_init() 系列
来源：http://tuz.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vpl.xziqi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vau.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ews.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ohb.xuetiantiany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://awc.fzhhl.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ccn.cashguo.top

================================================================================
来源：http://qxl.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境
来源：http://wvy.zhixingplan.top

================================================================================
来源：http://zac.hammf.cn

[M01] 读取命令行参数
来源：http://kce.sysykeji.top

Py:   sys.argv[1:]
来源：http://kwf.vqdsnc.cn

PHP:  $argv;  $argc;
来源：http://pek.tarul.cn

JS:   process.argv.slice(2)
来源：http://hpm.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://bjs.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://nil.dashuyun.cn

Go:   os.Args[1:]
来源：http://pnd.shanyushiyangkeji.top

Ruby: ARGV
来源：http://isa.shanyushiyangtech.top

C#:   args 数组（Main 方法参数）
来源：http://ycc.shanyushiyangkeji.top

[M02] 读取环境变量
来源：http://dja.redwolf501.top

Py:   os.environ.get("HOME")
来源：http://rpc.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://def.snrcjt.cn

JS:   process.env.HOME
来源：http://hvc.tarul.cn

TS:   process.env.HOME
来源：http://hhk.fktsv.cn

Java: System.getenv("HOME")
来源：http://jqa.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iqi.hcnkem.com

Ruby: ENV["HOME"]
来源：http://aqw.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nxi.hesvh.cn

[M03] 执行外部命令
来源：http://egn.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xup.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ipi.uphjek.com

JS:   child_process.execSync("ls -l").toString()
来源：http://rsy.ppjwa.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ptz.fktsv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hvs.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nvs.jinqigufen.top

Ruby: system("ls -l");  `ls -l`
来源：http://wxs.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://bfu.havefunace.top

[M04] 获取当前工作目录
来源：http://wfm.zhongyouzk.top

Py:   os.getcwd()
来源：http://jvv.jinqigfzy.top

PHP:  getcwd();
来源：http://pze.dashuyun.cn

JS:   process.cwd()
来源：http://uct.jinqigufen.top

TS:   process.cwd()
来源：http://bri.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://pfr.fzhhl.top

Go:   os.Getwd()
来源：http://mtt.gaohongyu789.top

Ruby: Dir.pwd
来源：http://rsb.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://krw.shzxlz.cn

[M05] 设置退出码
来源：http://vwy.svipenyu.cn

Py:   sys.exit(1)
来源：http://yzt.fktsv.cn

PHP:  exit(1);
来源：http://tng.zdqjudy.top

JS:   process.exit(1)
来源：http://uke.jinqigufen.top

TS:   process.exit(1)
来源：http://chv.bjfxy.top

Java: System.exit(1)
来源：http://wcp.dianchejie.cn

Go:   os.Exit(1)
来源：http://kis.chenjidiqi.icu

Ruby: exit 1
来源：http://dtn.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://asc.yfazqb.com

[M06] 向标准错误输出
来源：http://jyt.wangshuangyany.cn

Py:   print("err", file=sys.stderr)
来源：http://voh.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cge.shangyingyoupin.top

JS:   console.error("err")
来源：http://aur.nwbrower.top

TS:   console.error("err")
来源：http://iaf.yuanzhike.top

Java: System.err.println("err")
来源：http://stj.jlsjyb.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tvj.chenjidiqi.icu

Ruby: warn "err"
来源：http://abk.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://lxt.nanxinkj.top

[M07] 判断是否为主入口
来源：http://qcq.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://bos.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://amd.zhongyouzk.top

JS:   require.main === module
来源：http://lpe.chenlongwang.top

TS:   require.main === module
来源：http://zic.daxiang520.top

Java: public static void main(String[] args)
来源：http://rqu.sufxvd.cn

Go:   func main()
来源：http://zfu.pengpengdd.cyou

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hvb.cucudq.cn

C#:   static void Main(string[] args)
来源：http://kqg.yonumen.top

[M08] 获取系统与运行时信息
来源：http://yeg.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://ohd.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://lya.hesvh.cn

JS:   process.platform;  process.version
来源：http://dor.fanxiaobao.xyz

TS:   process.platform;  process.version
来源：http://pif.cashguo.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bqp.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jde.yongpay.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pbm.daria6918.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gfp.snrcjt.cn

================================================================================
来源：http://nxi.fengsongda.top

N. 数据结构与算法
来源：http://get.ivvv.top

================================================================================
来源：http://tpx.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://imk.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vgo.vqdsnc.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://asl.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pjn.mhx1999.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://owt.yvedp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jpq.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://euw.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jxj.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rae.iojbl.cn

[N02] 排序（工程实践用内置实现）
来源：http://tzn.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://ftp.cashguo.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kdt.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qav.xingfuxueyuan.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://cbm.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gcn.svipenyu.cn

Go:   slices.Sort(arr)
来源：http://fpl.epnwcf.com

Ruby: arr.sort
来源：http://opw.hcnkem.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://gdp.yangfankeji.com

[N03] 快速排序（分治示例）
来源：http://lvx.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lta.yueranfly.top


<!-- 参考信息 -->