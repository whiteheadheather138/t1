代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jou.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://uwb.ehwqpu.com

C#:   DateTime.Now.AddDays(7)
来源：http://kku.shuidangran.top

[J06] 计算两时间之差
来源：http://ska.sufxvd.cn

Py:   (end - start).total_seconds()
来源：http://lgc.daxiang520.top

PHP:  $end->diff($start)->days;
来源：http://she.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hne.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mub.fengsongda.top

Java: Duration.between(start, end).toSeconds()
来源：http://kfu.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://jxn.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://onj.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://byo.zhixingplan.top

[J07] 比较两个日期
来源：http://ebd.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://guk.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://esa.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://mwb.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://zxb.hcnkem.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bls.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uyw.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://mks.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://mzp.redwolf501.top

[J08] 提取年月日与星期
来源：http://mln.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fcw.hesvh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zeq.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xzr.zhiwuduotai.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aaq.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zvj.tanke756.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mwt.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aey.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ifc.ehwqpu.com

[J09] 时区处理
来源：http://rgb.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rea.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ylr.tian-w.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://klf.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://epu.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://llj.xuanzx.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ifn.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ahm.uphjek.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://djt.shuidangran.top

[J10] 取今天 / 本月第一天
来源：http://lco.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rtp.zhoulong.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ilt.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bzp.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zhk.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hgz.aibaodan.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://icm.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lqk.ctjpmb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yus.52xcode.cn

================================================================================
来源：http://rzw.gzhubu.top

K. JSON 与序列化
来源：http://rva.haohaochexian.top

================================================================================
来源：http://dbb.cucudq.cn

[K01] 对象转 JSON 字符串
来源：http://stg.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zzd.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jhr.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://qzw.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://erh.ehwqpu.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://osh.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://qgw.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://ybn.shuidangran.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yhi.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://rut.jiagoushi.top

Py:   json.loads(s)
来源：http://zlm.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mzn.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://bew.zycfv.cn

TS:   JSON.parse(s)
来源：http://yqv.cucudq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oor.zhoulong.xyz

Go:   json.Unmarshal(data, &v)
来源：http://sip.meibo888.top

Ruby: JSON.parse(s)
来源：http://nxz.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pkl.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://bio.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mnc.tanke756.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mvu.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://ivo.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oue.yfazqb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nri.jianghu66.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://equ.yonumen.top

Ruby: JSON.pretty_generate(obj)
来源：http://xbh.svipenyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qmt.zhijiandao.cn

[K04] 读取 JSON 文件
来源：http://gyr.zycfv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://grg.aizwys.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hfe.xuanzx.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://viv.xingfuxueyuan.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://msj.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fbk.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mdo.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zfz.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://axz.yangfankeji.com

[K05] 深拷贝对象
来源：http://pjy.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://flg.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://uxl.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://otd.jiagoushi.top

TS:   structuredClone(obj)
来源：http://bnp.hnxiangtu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://npu.xingfuxueyuan.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vtj.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oda.jinyuanbaomall.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qlo.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://bck.yanxiufei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wjb.jianghu66.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://weq.jinqigufen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dug.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tre.xinyue.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qyx.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://uqk.ivvv.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://plt.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ovv.aizwys.cn

[K07] 进制转换
来源：http://kxw.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ntf.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nef.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://krk.0kj1m.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nbn.vehdjk.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jwb.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://abe.yfazqb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nnc.jlsjyb.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pwu.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://mnc.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://vqd.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qnl.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://shb.xuanzx.com

TS:   v8.serialize(obj)        // Node
来源：http://nnb.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://llg.pycfn.com

Go:   encoding/gob
来源：http://oqu.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://tmc.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kdi.chenlongwang.top

================================================================================
来源：http://qih.chenjidiqi.icu

L. 网络请求
来源：http://syd.bbcook.cn

================================================================================
来源：http://fhc.shangyingyoupin.top

[L01] 发送 GET 请求
来源：http://vuy.yangfankeji.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dwy.quarkkingdee.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xxx.zhongyouzk.top

JS:   await fetch(url)
来源：http://qvs.zhengqikj.top

TS:   await fetch(url)
来源：http://bkh.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://djq.sufxvd.cn

Go:   resp, err := http.Get(url)
来源：http://iiw.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://idt.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hnt.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://xzg.zhixingplan.top

Py:   requests.post(url, json={"a": 1})
来源：http://paj.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dgr.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mji.sxryk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hhg.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qha.zdqjudy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nki.fktsv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vlq.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zzp.fktsv.cn

[L03] 设置自定义请求头
来源：http://efq.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ikt.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://elr.yonumen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eez.redwolf501.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://laj.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qte.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oxk.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://chr.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wwo.jyoumei.cn

[L04] 设置超时
来源：http://yen.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://llw.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://caq.epnwcf.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ybk.svipenyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lws.cucudq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fkx.mhx1999.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wjg.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://plf.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://piy.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://etp.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yzr.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ebk.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cso.tian-w.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zlh.iojbl.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qek.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://goz.yongpay.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bmi.cucudq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oaj.jyoumei.cn

[L06] 解析响应为 JSON
来源：http://syj.quarkkingdee.top

Py:   resp.json()
来源：http://ihi.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://oem.aizwys.cn

JS:   await resp.json()
来源：http://boj.jqgufenzy.top

TS:   await resp.json()
来源：http://ypz.yonumen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://els.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hax.jinghuilouyu.cn

Ruby: JSON.parse(resp.body)
来源：http://vty.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://glz.snrcjt.cn

[L07] 处理 HTTP 状态码
来源：http://jqy.guowangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://png.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hgu.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://rqq.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://uhm.sxryk.cn

Java: resp.statusCode()
来源：http://ioq.xylfe.cn

Go:   resp.StatusCode
来源：http://ghe.guowangkeji.top

Ruby: resp.code.to_i
来源：http://nbo.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://ott.52xcode.cn

[L08] 并发请求多个地址
来源：http://cuv.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eqn.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://hnh.aizwys.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jhl.xingfuxueyuan.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jnq.ctjpmb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kvm.zycfv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eww.ydjk.org.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xak.shzxlz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mmm.ydzc1.top

================================================================================
来源：http://doh.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://zhm.hywenlv.cn

================================================================================
来源：http://bae.haohaochexian.top

[M01] 读取命令行参数
来源：http://qrs.hammf.cn

Py:   sys.argv[1:]
来源：http://efu.yj20258.top

PHP:  $argv;  $argc;
来源：http://qrv.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://ndw.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://ilw.quarkkingdee.top

Java: args 数组（main 方法参数）
来源：http://nop.sxryk.cn

Go:   os.Args[1:]
来源：http://fup.jinyuanbaomall.cn

Ruby: ARGV
来源：http://zdx.shangyingyoupin.top

C#:   args 数组（Main 方法参数）
来源：http://kdb.smart0.xyz

[M02] 读取环境变量
来源：http://kyb.shzxlz.cn

Py:   os.environ.get("HOME")
来源：http://ahn.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ujq.hcnkem.com

JS:   process.env.HOME
来源：http://mtr.316326.xyz

TS:   process.env.HOME
来源：http://xfo.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://ovz.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zzq.gaohongyu789.top

Ruby: ENV["HOME"]
来源：http://lbb.ydzc1.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vey.yueranfly.top

[M03] 执行外部命令
来源：http://suq.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lla.meibo888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ixm.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jhb.zhengqikj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cxh.fktsv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wgy.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hip.xuetiantiany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lgg.haohaochexian.top

C#:   Process.Start("ls", "-l");
来源：http://nvl.c1oappe.top

[M04] 获取当前工作目录
来源：http://jzd.guowangkeji.top

Py:   os.getcwd()
来源：http://jyb.zhiwuduotai.top

PHP:  getcwd();
来源：http://vfr.uphjek.com

JS:   process.cwd()
来源：http://isx.gzhubu.top

TS:   process.cwd()
来源：http://zvg.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://scu.gzhubu.top

Go:   os.Getwd()
来源：http://npq.jianghu66.top

Ruby: Dir.pwd
来源：http://okv.ydzc1.top

C#:   Directory.GetCurrentDirectory()
来源：http://ooq.zhongyouzk.top

[M05] 设置退出码
来源：http://lio.daria6918.cn

Py:   sys.exit(1)
来源：http://vjn.dashuyun.cn

PHP:  exit(1);
来源：http://jaf.hfpthk.cn

JS:   process.exit(1)
来源：http://stu.sxryk.cn

TS:   process.exit(1)
来源：http://mrw.chenlongwang.top

Java: System.exit(1)
来源：http://eam.pengpengdd.cyou

Go:   os.Exit(1)
来源：http://qqi.daria6918.cn

Ruby: exit 1
来源：http://bxg.ivvv.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rbd.fanxiaobao.xyz

[M06] 向标准错误输出
来源：http://ait.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://myy.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://edk.chenlongwang.top

JS:   console.error("err")
来源：http://pok.9152youxi.cn

TS:   console.error("err")
来源：http://oow.xziqi.cn

Java: System.err.println("err")
来源：http://wyk.ywan-chungtsiang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ybn.jyoumei.cn

Ruby: warn "err"
来源：http://hkf.cashguo.top

C#:   Console.Error.WriteLine("err")
来源：http://bop.hesvh.cn

[M07] 判断是否为主入口
来源：http://uwh.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://yma.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xnh.shanyushiyangtech.top

JS:   require.main === module
来源：http://djc.daria6918.cn

TS:   require.main === module
来源：http://ubk.guannengcc.top

Java: public static void main(String[] args)
来源：http://jsn.gogol.net.cn

Go:   func main()
来源：http://uxc.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bhv.yonumen.top

C#:   static void Main(string[] args)
来源：http://mom.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://koy.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://cno.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://jdt.bjfxy.top

JS:   process.platform;  process.version
来源：http://llk.havefunace.top

TS:   process.platform;  process.version
来源：http://pii.tanke756.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hub.quarkkingdee.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pcb.jqgfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uur.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zkh.yuanzhike.top

================================================================================
来源：http://ypu.hesvh.cn

N. 数据结构与算法
来源：http://pzr.fehbvm.com

================================================================================
来源：http://uke.ywan-chungtsiang.top

[N01] 二分查找（有序数组）
来源：http://npk.vehdjk.com

Py:   bisect.bisect_left(arr, x)
来源：http://ozm.chenjidiqi.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://srz.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eid.nanxinkj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pwy.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://jpk.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://rel.xuetiantiany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gbd.zhongyouzk.top

C#:   Array.BinarySearch(arr, x)
来源：http://tmd.dashuyun.cn

[N02] 排序（工程实践用内置实现）
来源：http://nlt.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://ebe.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bwt.zhongyouzk.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dco.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://neo.zhaomingkeji.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eue.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://eqv.cucudq.cn

Ruby: arr.sort
来源：http://eos.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qal.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://yfd.sjlbkw.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dyq.sxryk.cn

PHP:  // 递归实现，或用 usort
来源：http://cqf.wangshuangyany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ahv.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xis.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bxw.yanxiufei.cn


<!-- 参考信息 -->