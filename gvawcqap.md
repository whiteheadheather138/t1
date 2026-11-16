代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kbe.yueranfly.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gpf.xziqi.cn

[J05] 时间加减（加 7 天）
来源：http://lyd.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://ywz.redwolf501.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cyj.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tny.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xcc.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://lph.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vjv.hongshengwenyu.top

Ruby: Time.now + 7 * 86400
来源：http://ijj.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gaq.sufxvd.cn

[J06] 计算两时间之差
来源：http://jpy.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://mzv.yanxiufei.cn

PHP:  $end->diff($start)->days;
来源：http://yen.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vhu.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cnd.jqgufenzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://vzi.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://zge.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://zad.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://ygy.yongpay.top

[J07] 比较两个日期
来源：http://ggh.xuetiantiany.cn

Py:   d1 < d2;  d1 == d2
来源：http://bkb.sufxvd.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://obu.zhengqikj.top

JS:   d1.getTime() < d2.getTime()
来源：http://zqk.aizwys.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mid.fktsv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dte.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dqz.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://vma.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://gaw.cqqwz.cn

[J08] 提取年月日与星期
来源：http://xyy.feifeiyinyue.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ydt.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yhb.pycfn.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ytz.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cuh.cashguo.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kky.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://scu.sxryk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xcl.hongshengwenyu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://evr.shanyushiyangkeji.top

[J09] 时区处理
来源：http://aqh.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://awi.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nsu.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lqr.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zjh.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eyb.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tsp.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://eoq.gzhubu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dtz.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://vky.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://pxv.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nrl.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wzc.yuanzhike.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kky.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ybx.yuanzhike.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tcj.meibo888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kjj.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lnc.fktsv.cn

================================================================================
来源：http://uwe.iojbl.cn

K. JSON 与序列化
来源：http://exz.hywenlv.cn

================================================================================
来源：http://xpu.mhx1999.top

[K01] 对象转 JSON 字符串
来源：http://mgs.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xrz.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gvv.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://okg.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://iri.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dfm.chenzaomai.com

Go:   json.Marshal(obj)
来源：http://tvm.zycfv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://utp.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://idl.sweek.top

[K02] JSON 字符串转对象
来源：http://ork.52xcode.cn

Py:   json.loads(s)
来源：http://rsc.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tly.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://yzg.guowangkeji.top

TS:   JSON.parse(s)
来源：http://hod.nwbrower.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fgq.xuanzx.com

Go:   json.Unmarshal(data, &v)
来源：http://pbu.hnqzz.top

Ruby: JSON.parse(s)
来源：http://cio.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kxp.shuidangran.top

[K03] JSON 美化输出（带缩进）
来源：http://orw.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aaa.tanke756.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rhb.yfazqb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://ovt.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zgr.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qnw.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qfa.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://myf.fengsongda.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nvg.xylfe.cn

[K04] 读取 JSON 文件
来源：http://xwg.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lid.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://giv.zhengqikj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jpt.jiagoushi.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gtx.yj20258888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tyw.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aip.bjfxy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dzu.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rvn.jyoumei.cn

[K05] 深拷贝对象
来源：http://yck.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://ftm.kuanghao11.cn

PHP:  unserialize(serialize($obj));
来源：http://ibe.hnxiangtu.top

JS:   structuredClone(obj)
来源：http://rej.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://jde.yuanzhike.top

Java: // 手写拷贝构造，或序列化往返
来源：http://snd.gogol.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rwf.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ikr.jinqigufen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://swv.fzhhl.top

[K06] 解析 URL 查询串
来源：http://plm.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qcy.dianchejie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dkc.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qxf.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://arf.svipenyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wqh.hnqzz.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vnx.chenjidiqi.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pmh.wangdashe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lke.bbcook.cn

[K07] 进制转换
来源：http://zvo.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://juc.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vew.wangshuangyany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nvr.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://poz.c1oappe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qqe.xingfuxueyuan.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://psk.cucudq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://syp.ywan-chungtsiang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xgv.ydjk.org.cn

[K08] 二进制序列化（非 JSON）
来源：http://nhf.bbcook.cn

Py:   pickle.dumps(obj)
来源：http://hyu.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rse.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://feu.pycfn.com

TS:   v8.serialize(obj)        // Node
来源：http://kpm.zhiwuduotai.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zth.ydzc1.top

Go:   encoding/gob
来源：http://rub.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://uay.dashuyun.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jwm.zhaomingkeji.xyz

================================================================================
来源：http://sjv.cashguo.top

L. 网络请求
来源：http://ebd.xuetiantiany.cn

================================================================================
来源：http://uvx.dashuyun.cn

[L01] 发送 GET 请求
来源：http://xvn.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nhc.jinyuanbaomall.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ldx.gogol.net.cn

JS:   await fetch(url)
来源：http://jhm.jinghuilouyu.cn

TS:   await fetch(url)
来源：http://yuf.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lpq.jqgfzy.top

Go:   resp, err := http.Get(url)
来源：http://ozv.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ctt.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jnn.yfazqb.com

[L02] 发送 POST JSON
来源：http://opu.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://zdf.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ldu.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vwq.xuetiantiany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://srp.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kko.zdbjq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://avm.ctjpmb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ghr.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://siq.c1oappe.top

[L03] 设置自定义请求头
来源：http://uhb.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mnd.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fph.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lqx.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iew.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rni.fengsongda.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://boc.wangshuangyany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://isl.hesvh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fpt.sweek.top

[L04] 设置超时
来源：http://dkc.cqqwz.cn

Py:   requests.get(url, timeout=5)
来源：http://ynt.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vdq.hnqzz.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vxl.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iuc.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sja.vehdjk.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jqx.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kky.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vjr.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://zms.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uym.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nrq.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kzf.tianlin.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://urk.meibo888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dha.jinyuanbaomall.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jor.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cdm.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lmi.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://yio.nanxinkj.top

Py:   resp.json()
来源：http://xnm.hammf.cn

PHP:  json_decode($body, true);
来源：http://qrt.sxryk.cn

JS:   await resp.json()
来源：http://koq.zycfv.cn

TS:   await resp.json()
来源：http://duo.sjlbkw.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://feq.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ylu.uphjek.com

Ruby: JSON.parse(resp.body)
来源：http://qjj.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vyu.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://mkg.hywenlv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uwq.hnqzz.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zqq.yfazqb.com

JS:   resp.ok;  resp.status
来源：http://pao.cucudq.cn

TS:   resp.ok;  resp.status
来源：http://vdw.yj20258.top

Java: resp.statusCode()
来源：http://vdt.zdqjudy.top

Go:   resp.StatusCode
来源：http://emi.wangdashe.top

Ruby: resp.code.to_i
来源：http://cyo.jinqigfzy.top

C#:   (int)resp.StatusCode
来源：http://sji.52xcode.cn

[L08] 并发请求多个地址
来源：http://rue.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://avu.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://epx.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zaf.hnxiangtu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mxs.meibo888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fyt.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ian.wangdashe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mtf.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wnv.pycfn.com

================================================================================
来源：http://aqm.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://htr.hfpthk.cn

================================================================================
来源：http://zhm.yonumen.top

[M01] 读取命令行参数
来源：http://csq.bbcook.cn

Py:   sys.argv[1:]
来源：http://jnj.hfpthk.cn

PHP:  $argv;  $argc;
来源：http://byp.0kj1m.cn

JS:   process.argv.slice(2)
来源：http://tym.daria6918.cn

TS:   process.argv.slice(2)
来源：http://jkm.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://hxv.shangyingyoupin.top

Go:   os.Args[1:]
来源：http://qju.sweek.top

Ruby: ARGV
来源：http://jhm.hnxiangtu.top

C#:   args 数组（Main 方法参数）
来源：http://nnz.c1oappe.top

[M02] 读取环境变量
来源：http://ndy.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://dxt.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://opt.snrcjt.cn

JS:   process.env.HOME
来源：http://vpa.daxiang520.top

TS:   process.env.HOME
来源：http://lbx.yvedp.cn

Java: System.getenv("HOME")
来源：http://lsh.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jxj.shanyushiyangtech.top

Ruby: ENV["HOME"]
来源：http://huh.iojbl.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://twj.jianghu66.top

[M03] 执行外部命令
来源：http://lph.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://giw.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rxi.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pql.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cjq.ctjpmb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gqw.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://het.jiagoushi.top

Ruby: system("ls -l");  `ls -l`
来源：http://clx.sjlbkw.cn

C#:   Process.Start("ls", "-l");
来源：http://knq.tianlin.xyz

[M04] 获取当前工作目录
来源：http://tju.hfpthk.cn

Py:   os.getcwd()
来源：http://mrg.fehbvm.com

PHP:  getcwd();
来源：http://mpu.bbcook.cn

JS:   process.cwd()
来源：http://tvz.daxiang520.top

TS:   process.cwd()
来源：http://rrp.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://qiv.ybcxt.top

Go:   os.Getwd()
来源：http://luv.gogol.net.cn

Ruby: Dir.pwd
来源：http://kxv.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://npg.aizwys.cn

[M05] 设置退出码
来源：http://mtf.jiagoushi.top

Py:   sys.exit(1)
来源：http://jmb.pycfn.com

PHP:  exit(1);
来源：http://iwy.xuetiantiany.cn

JS:   process.exit(1)
来源：http://loh.tanke756.top

TS:   process.exit(1)
来源：http://igb.nwbrower.top

Java: System.exit(1)
来源：http://tbg.zhixingplan.top

Go:   os.Exit(1)
来源：http://oht.yvedp.cn

Ruby: exit 1
来源：http://cvs.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://myr.jinqigfzy.top

[M06] 向标准错误输出
来源：http://oql.fengsongda.top

Py:   print("err", file=sys.stderr)
来源：http://rjv.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dax.zhijiandao.cn

JS:   console.error("err")
来源：http://bvn.ybcxt.top

TS:   console.error("err")
来源：http://kxl.feifeiyinyue.top

Java: System.err.println("err")
来源：http://ztc.smart0.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ysl.fanxiaobao.xyz

Ruby: warn "err"
来源：http://amo.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://gev.yvedp.cn

[M07] 判断是否为主入口
来源：http://usi.yfazqb.com

Py:   if __name__ == "__main__":
来源：http://npd.kuanghao11.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eyq.cucudq.cn

JS:   require.main === module
来源：http://kxo.wangshuangyany.cn

TS:   require.main === module
来源：http://qac.hnxiangtu.top

Java: public static void main(String[] args)
来源：http://dmo.gotoacloud.top

Go:   func main()
来源：http://rtl.pengpengdd.cyou

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ybp.bbcook.cn

C#:   static void Main(string[] args)
来源：http://xnd.yongpay.top

[M08] 获取系统与运行时信息
来源：http://jjn.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://vfo.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://kme.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://pgj.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://axv.zhengqikj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bdm.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nrs.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://evf.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://xsh.svipenyu.cn

================================================================================
来源：http://rlf.mhx1999.top

N. 数据结构与算法
来源：http://cmx.52xcode.cn

================================================================================
来源：http://yqd.ydzc1.top

[N01] 二分查找（有序数组）
来源：http://lbj.hfpthk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vrn.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jex.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wgg.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gca.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xwq.feifeiyinyue.top

Go:   sort.SearchInts(arr, x)
来源：http://fge.xylfe.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vtx.jinqigfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://umg.iojbl.cn

[N02] 排序（工程实践用内置实现）
来源：http://zen.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://unu.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jcf.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://vtz.epnwcf.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://cgv.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://peh.sxryk.cn

Go:   slices.Sort(arr)
来源：http://rag.hfpthk.cn


<!-- 参考信息 -->