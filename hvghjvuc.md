代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://urd.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://pqq.kuanghao11.cn

C#:   DateTime.Now.AddDays(7)
来源：http://suu.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://xaf.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://ldf.ivvv.top

PHP:  $end->diff($start)->days;
来源：http://afy.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ama.jqgfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://agk.shanyushiyangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://fxb.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://mpd.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://iah.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://ivl.ywan-chungtsiang.top

[J07] 比较两个日期
来源：http://puz.zycfv.cn

Py:   d1 < d2;  d1 == d2
来源：http://myj.guowangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ktm.fehbvm.com

JS:   d1.getTime() < d2.getTime()
来源：http://ugi.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://nsr.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lwy.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ozf.yj202588.top

Ruby: d1 < d2;  d1 == d2
来源：http://syx.xinyue.icu

C#:   d1 < d2;  d1 == d2
来源：http://bjv.jqgfzy.top

[J08] 提取年月日与星期
来源：http://efj.iojbl.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iyo.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://evx.jyoumei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ftc.sjlbkw.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mrm.shangyingyoupin.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jvt.tanke756.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gpo.jinyuanbaomall.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jsj.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cex.daxiang520.top

[J09] 时区处理
来源：http://vbz.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zri.fktsv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kjf.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ens.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hlr.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qyv.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mtq.fehbvm.com

Ruby: Time.now.getlocal("+08:00")
来源：http://jrg.uphjek.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ofv.ywan-chungtsiang.top

[J10] 取今天 / 本月第一天
来源：http://fhf.xinyue.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://bfe.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ird.yj20258888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qyw.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qvf.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bvb.zhengqikj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tia.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ozo.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tzr.cashguo.top

================================================================================
来源：http://qmf.xuetiantiany.cn

K. JSON 与序列化
来源：http://vdz.gogol.net.cn

================================================================================
来源：http://lom.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://vtp.ivvv.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bxb.aibaodan.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ebn.xziqi.cn

JS:   JSON.stringify(obj)
来源：http://vpt.yongpay.top

TS:   JSON.stringify(obj)
来源：http://bci.c1oappe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://adh.zhoulong.xyz

Go:   json.Marshal(obj)
来源：http://vto.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hau.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gtj.aizwys.cn

[K02] JSON 字符串转对象
来源：http://sug.shzxlz.cn

Py:   json.loads(s)
来源：http://fqp.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eyz.cqqwz.cn

JS:   JSON.parse(s)
来源：http://mcw.hywenlv.cn

TS:   JSON.parse(s)
来源：http://oxx.cheryme.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vce.hfpthk.cn

Go:   json.Unmarshal(data, &v)
来源：http://ebl.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://aar.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hkx.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://tbl.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://obz.hongshengwenyu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eng.tian-w.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uyv.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gdt.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://flc.birdmap.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mky.nwbrower.top

Ruby: JSON.pretty_generate(obj)
来源：http://zvu.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://spz.gogol.net.cn

[K04] 读取 JSON 文件
来源：http://sys.feifeiyinyue.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ejm.svipenyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ftb.svipenyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://abk.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tuu.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ycr.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bfr.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kao.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kog.xylfe.cn

[K05] 深拷贝对象
来源：http://mlp.sxryk.cn

Py:   copy.deepcopy(obj)
来源：http://aoj.xinyue.icu

PHP:  unserialize(serialize($obj));
来源：http://pfl.c1oappe.top

JS:   structuredClone(obj)
来源：http://ono.cashguo.top

TS:   structuredClone(obj)
来源：http://hgm.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gza.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qrh.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mse.sysykeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vds.ybcxt.top

[K06] 解析 URL 查询串
来源：http://srz.zhongyouzk.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fay.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zzk.yj20258.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mda.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ila.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pzl.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://znc.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qrb.smart0.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zqk.shuidangran.top

[K07] 进制转换
来源：http://yfy.iojbl.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ikb.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://myu.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ezr.dashuyun.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zat.dashuyun.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yhn.hnqzz.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nsk.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://isk.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fox.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://lri.aibaodan.cn

Py:   pickle.dumps(obj)
来源：http://gbs.yangfankeji.com

PHP:  serialize($obj);  unserialize($s);
来源：http://yqd.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://icd.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://qhn.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xej.yuanzhike.top

Go:   encoding/gob
来源：http://umi.hfpthk.cn

Ruby: Marshal.dump(obj)
来源：http://vkm.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mhz.vqdsnc.cn

================================================================================
来源：http://zgv.jqgfzy.top

L. 网络请求
来源：http://uho.0kj1m.cn

================================================================================
来源：http://xev.jinqigfzy.top

[L01] 发送 GET 请求
来源：http://rlx.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qnk.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mmk.tanke756.top

JS:   await fetch(url)
来源：http://hsc.wangshuangyany.cn

TS:   await fetch(url)
来源：http://mxl.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lhp.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://ezr.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kbw.52xcode.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xcp.havefunace.top

[L02] 发送 POST JSON
来源：http://oqv.nanxuanxn.top

Py:   requests.post(url, json={"a": 1})
来源：http://neq.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uhw.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ugx.yfazqb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kci.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zgd.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pgi.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ypn.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wxb.jlsjyb.cn

[L03] 设置自定义请求头
来源：http://gzs.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vit.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ixp.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://adc.chenzaomai.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zjb.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://klv.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lkz.chenzaomai.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tms.iojbl.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yei.jiagoushi.top

[L04] 设置超时
来源：http://ppj.ppjwa.cn

Py:   requests.get(url, timeout=5)
来源：http://wrd.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ocb.haohaochexian.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vpz.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vsr.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ihx.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cvb.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://djl.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cww.fanxiaobao.xyz

[L05] 上传文件（multipart）
来源：http://uts.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hvx.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ngr.uphjek.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cxu.shanyushiyangtech.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://prk.gaohongyu789.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kxh.52xcode.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://umk.meibo888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jvl.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mph.haohaochexian.top

[L06] 解析响应为 JSON
来源：http://ztp.zhiwuduotai.top

Py:   resp.json()
来源：http://bhe.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://tsq.jqgfzy.top

JS:   await resp.json()
来源：http://pvo.fengsongda.top

TS:   await resp.json()
来源：http://eff.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xyh.sjlbkw.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xss.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://yyi.hysaishi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ycs.zhoulong.xyz

[L07] 处理 HTTP 状态码
来源：http://kfa.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://elm.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bvw.redwolf501.top

JS:   resp.ok;  resp.status
来源：http://xjd.gzhubu.top

TS:   resp.ok;  resp.status
来源：http://djg.zdbjq.cn

Java: resp.statusCode()
来源：http://qbk.jinyuanbaomall.cn

Go:   resp.StatusCode
来源：http://axf.wangshuangyany.cn

Ruby: resp.code.to_i
来源：http://avd.uphjek.com

C#:   (int)resp.StatusCode
来源：http://icv.zycfv.cn

[L08] 并发请求多个地址
来源：http://qwk.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eav.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://rzx.zdqjudy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ubv.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pzn.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uli.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dsd.zhiwuduotai.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ekn.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fhm.shzxlz.cn

================================================================================
来源：http://ofb.bjfxy.top

M. 命令行 / 进程 / 环境
来源：http://dax.sweek.top

================================================================================
来源：http://uxs.tianlin.xyz

[M01] 读取命令行参数
来源：http://fec.shanyushiyangtech.top

Py:   sys.argv[1:]
来源：http://dnf.aizwys.cn

PHP:  $argv;  $argc;
来源：http://meu.fzhhl.top

JS:   process.argv.slice(2)
来源：http://vec.jinqigufen.top

TS:   process.argv.slice(2)
来源：http://voh.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://qyi.xziqi.cn

Go:   os.Args[1:]
来源：http://axy.jqgfzy.top

Ruby: ARGV
来源：http://mck.guowangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://pep.guowangkeji.top

[M02] 读取环境变量
来源：http://jth.zhixingplan.top

Py:   os.environ.get("HOME")
来源：http://emg.jiagoushi.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bte.dianchejie.cn

JS:   process.env.HOME
来源：http://hia.jiagoushi.top

TS:   process.env.HOME
来源：http://wgt.cucudq.cn

Java: System.getenv("HOME")
来源：http://vfo.tianlin.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lmz.chenjidiqi.icu

Ruby: ENV["HOME"]
来源：http://rhv.xinyue.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xde.fktsv.cn

[M03] 执行外部命令
来源：http://csy.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ssq.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tms.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://csk.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ili.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yim.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ibj.chenlongwang.top

Ruby: system("ls -l");  `ls -l`
来源：http://ccq.sxryk.cn

C#:   Process.Start("ls", "-l");
来源：http://gbe.yuxming.cn

[M04] 获取当前工作目录
来源：http://sbz.zhaomingkeji.xyz

Py:   os.getcwd()
来源：http://pja.sjlbkw.cn

PHP:  getcwd();
来源：http://hsg.uphjek.com

JS:   process.cwd()
来源：http://poe.sweek.top

TS:   process.cwd()
来源：http://ods.shzxlz.cn

Java: Path.of("").toAbsolutePath()
来源：http://vtm.zhengqikj.top

Go:   os.Getwd()
来源：http://ulr.cdnleiting.top

Ruby: Dir.pwd
来源：http://qcy.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://cvh.chenlongwang.top

[M05] 设置退出码
来源：http://qsl.hesvh.cn

Py:   sys.exit(1)
来源：http://pcx.ybcxt.top

PHP:  exit(1);
来源：http://fuu.ybcxt.top

JS:   process.exit(1)
来源：http://iad.haohaochexian.top

TS:   process.exit(1)
来源：http://lwl.bjfxy.top

Java: System.exit(1)
来源：http://fvk.guowangkeji.top

Go:   os.Exit(1)
来源：http://eez.tianlin.xyz

Ruby: exit 1
来源：http://peq.guannengcc.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://trr.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://duj.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://qnl.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mcp.xylfe.cn

JS:   console.error("err")
来源：http://wlc.nwbrower.top

TS:   console.error("err")
来源：http://peb.yanxiufei.cn

Java: System.err.println("err")
来源：http://ahz.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bkp.yuanzhike.top

Ruby: warn "err"
来源：http://yds.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://nkc.cucudq.cn

[M07] 判断是否为主入口
来源：http://rjy.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://nea.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gtq.yangfankeji.com

JS:   require.main === module
来源：http://hdl.9152youxi.cn

TS:   require.main === module
来源：http://jaz.zhengqikj.top

Java: public static void main(String[] args)
来源：http://lkq.zycfv.cn

Go:   func main()
来源：http://vvu.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mur.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://vzu.snrcjt.cn

[M08] 获取系统与运行时信息
来源：http://mqk.meibo888.top

Py:   platform.system();  platform.python_version()
来源：http://guh.fzhhl.top

PHP:  PHP_OS;  phpversion();
来源：http://cgi.svipenyu.cn

JS:   process.platform;  process.version
来源：http://yir.xuanzx.com

TS:   process.platform;  process.version
来源：http://ube.shanyushiyangtech.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fgh.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://eth.tianlin.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nyt.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://odb.xylfe.cn

================================================================================
来源：http://eiq.shanyushiyangtech.top

N. 数据结构与算法
来源：http://xvk.vehdjk.com

================================================================================
来源：http://aqi.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://gfd.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kst.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://khh.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fce.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://duh.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://nyu.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://sxb.yongpay.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mna.sjlbkw.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bhe.zhengqikj.top

[N02] 排序（工程实践用内置实现）
来源：http://pki.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://jfv.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fsi.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qpa.yvedp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hwb.shangyingyoupin.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://une.daria6918.cn

Go:   slices.Sort(arr)
来源：http://ksi.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://znc.cucudq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vfr.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://qgx.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mli.shuidangran.top

PHP:  // 递归实现，或用 usort
来源：http://xbv.c1oappe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zvn.fktsv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yir.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nki.yfazqb.com


<!-- 参考信息 -->