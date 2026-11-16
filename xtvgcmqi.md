代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://sjb.sysykeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://enb.sxryk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zef.jinqigufen.top

Java: LocalDate.now().plusDays(7)
来源：http://iyp.vehdjk.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qbf.bbcook.cn

Ruby: Time.now + 7 * 86400
来源：http://pls.316326.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ddh.smart0.xyz

[J06] 计算两时间之差
来源：http://jqx.havefunace.top

Py:   (end - start).total_seconds()
来源：http://fjw.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://mvn.zhengqikj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sou.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ktm.yanxiufei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aoe.hongshengwenyu.top

Go:   end.Sub(start).Hours()
来源：http://mbp.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://zsw.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://efn.yueranfly.top

[J07] 比较两个日期
来源：http://acx.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://ucs.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qkj.ydjk.org.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oze.yj202588.top

TS:   d1.getTime() < d2.getTime()
来源：http://qib.smart0.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nmk.sysykeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vva.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dlh.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://csg.zhaomingkeji.xyz

[J08] 提取年月日与星期
来源：http://ezn.ivvv.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mdh.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gjv.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jxu.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uvx.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ysz.hysaishi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xit.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dzr.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mka.zhengqikj.top

[J09] 时区处理
来源：http://lod.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gtj.zhijiandao.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://amx.cdnleiting.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rid.haohaochexian.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mpk.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jci.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ypv.ydzc1.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qdt.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mkg.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://hrk.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gkt.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nbu.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://emf.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ykc.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zyq.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cyv.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yit.chenzaomai.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jwl.316326.xyz

================================================================================
来源：http://qul.hywenlv.cn

K. JSON 与序列化
来源：http://dcb.jqgfzy.top

================================================================================
来源：http://jmx.jinqigufen.top

[K01] 对象转 JSON 字符串
来源：http://rfn.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://heu.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://whl.hysaishi.cn

JS:   JSON.stringify(obj)
来源：http://lsd.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://eto.uphjek.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://was.zdqjudy.top

Go:   json.Marshal(obj)
来源：http://fic.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://yws.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cav.tian-w.cn

[K02] JSON 字符串转对象
来源：http://utk.xuetiantiany.cn

Py:   json.loads(s)
来源：http://tyg.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://err.hfpthk.cn

JS:   JSON.parse(s)
来源：http://zew.52xcode.cn

TS:   JSON.parse(s)
来源：http://vbw.feifeiyinyue.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wzf.gogol.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://otj.zdqjudy.top

Ruby: JSON.parse(s)
来源：http://yga.uphjek.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lxg.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://veu.dianchejie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xas.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fcs.hammf.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qlg.snrcjt.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bsy.zycfv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ztq.jinghuilouyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hjk.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://npi.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sib.vqdsnc.cn

[K04] 读取 JSON 文件
来源：http://heg.nanxuanxn.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://phm.snrcjt.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zhd.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oqc.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sfi.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xym.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vlu.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://naz.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://okf.sweek.top

[K05] 深拷贝对象
来源：http://mua.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://nne.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://zjw.svipenyu.cn

JS:   structuredClone(obj)
来源：http://fee.iojbl.cn

TS:   structuredClone(obj)
来源：http://iuw.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://car.zhijiandao.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tml.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nnx.ctjpmb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://klq.ydjk.org.cn

[K06] 解析 URL 查询串
来源：http://ioj.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xva.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dzj.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ngu.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qii.zhoulong.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://afj.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yim.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dnn.andypj.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eni.daxiang520.top

[K07] 进制转换
来源：http://rso.cashguo.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uwq.xingfuxueyuan.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://swp.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vly.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hkr.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hrq.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sig.epnwcf.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iov.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cft.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://cie.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://fag.hcnkem.com

PHP:  serialize($obj);  unserialize($s);
来源：http://anf.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://umw.zycfv.cn

TS:   v8.serialize(obj)        // Node
来源：http://bcf.fktsv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dso.jinqigufen.top

Go:   encoding/gob
来源：http://fjz.jiagoushi.top

Ruby: Marshal.dump(obj)
来源：http://pfo.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xbr.c1oappe.top

================================================================================
来源：http://kpk.cashguo.top

L. 网络请求
来源：http://dpx.c1oappe.top

================================================================================
来源：http://zjp.hfpthk.cn

[L01] 发送 GET 请求
来源：http://oti.zhongyouzk.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://paf.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ueg.shzxlz.cn

JS:   await fetch(url)
来源：http://mfj.nanxuanxn.top

TS:   await fetch(url)
来源：http://ysl.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tff.sufxvd.cn

Go:   resp, err := http.Get(url)
来源：http://lhu.hywenlv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kny.shuidangran.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gul.fzhhl.top

[L02] 发送 POST JSON
来源：http://bct.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://wpr.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bki.shuidangran.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pbd.yvedp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cmp.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mpb.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://asm.smart0.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bay.yj20258888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://szp.jiagoushi.top

[L03] 设置自定义请求头
来源：http://ljk.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://esr.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xhb.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zbn.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://scl.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zic.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zah.fzhhl.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://syg.xuetiantiany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jpr.pycfn.com

[L04] 设置超时
来源：http://hpi.gogol.net.cn

Py:   requests.get(url, timeout=5)
来源：http://cmc.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eno.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pff.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vdc.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yir.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aik.cdnleiting.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bnz.tianlin.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://frv.daxiang520.top

[L05] 上传文件（multipart）
来源：http://lkr.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dkg.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gzl.gotoacloud.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pcg.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ref.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dbu.vqdsnc.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rty.sweek.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jxt.316326.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lto.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://hdi.fengsongda.top

Py:   resp.json()
来源：http://jmz.zhengqikj.top

PHP:  json_decode($body, true);
来源：http://qoe.smart0.xyz

JS:   await resp.json()
来源：http://mja.hcnkem.com

TS:   await resp.json()
来源：http://zqj.yvedp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hsx.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kxi.meibo888.top

Ruby: JSON.parse(resp.body)
来源：http://bxr.hongshengwenyu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vxb.bbcook.cn

[L07] 处理 HTTP 状态码
来源：http://bys.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fan.pycfn.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xtp.52xcode.cn

JS:   resp.ok;  resp.status
来源：http://edd.fehbvm.com

TS:   resp.ok;  resp.status
来源：http://afx.sxryk.cn

Java: resp.statusCode()
来源：http://cfx.redwolf501.top

Go:   resp.StatusCode
来源：http://ogt.haohaochexian.top

Ruby: resp.code.to_i
来源：http://upp.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://uvf.ivvv.top

[L08] 并发请求多个地址
来源：http://xws.sysykeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ong.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://sai.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://grz.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ocg.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ool.fanxiaobao.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://max.yj20258888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://its.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tnz.c1oappe.top

================================================================================
来源：http://byw.tanke756.top

M. 命令行 / 进程 / 环境
来源：http://tam.feifeiyinyue.top

================================================================================
来源：http://jjj.dianchejie.cn

[M01] 读取命令行参数
来源：http://ggq.epnwcf.com

Py:   sys.argv[1:]
来源：http://sxe.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://kyg.chenlongwang.top

JS:   process.argv.slice(2)
来源：http://gmp.gogol.net.cn

TS:   process.argv.slice(2)
来源：http://gms.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://lcf.xylfe.cn

Go:   os.Args[1:]
来源：http://sze.tian-w.cn

Ruby: ARGV
来源：http://lkw.daxiang520.top

C#:   args 数组（Main 方法参数）
来源：http://zmn.daria6918.cn

[M02] 读取环境变量
来源：http://kde.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://idj.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tds.birdmap.top

JS:   process.env.HOME
来源：http://vex.fehbvm.com

TS:   process.env.HOME
来源：http://urf.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://wqe.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ybt.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://ukj.jinghuilouyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dke.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://hqu.snrcjt.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mdk.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://man.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fpc.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://adj.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vcp.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hmy.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://jxx.yongpay.top

C#:   Process.Start("ls", "-l");
来源：http://pmh.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://oii.sufxvd.cn

Py:   os.getcwd()
来源：http://bri.ppjwa.cn

PHP:  getcwd();
来源：http://cza.haohaochexian.top

JS:   process.cwd()
来源：http://ibu.daxiang520.top

TS:   process.cwd()
来源：http://emk.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://dki.jlsjyb.cn

Go:   os.Getwd()
来源：http://zmv.jianghu66.top

Ruby: Dir.pwd
来源：http://vfq.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xut.zhoulong.xyz

[M05] 设置退出码
来源：http://ekw.jinghuilouyu.cn

Py:   sys.exit(1)
来源：http://wnb.xuetiantiany.cn

PHP:  exit(1);
来源：http://ney.dashuyun.cn

JS:   process.exit(1)
来源：http://nwh.zycfv.cn

TS:   process.exit(1)
来源：http://key.c1oappe.top

Java: System.exit(1)
来源：http://gdw.dianchejie.cn

Go:   os.Exit(1)
来源：http://fcr.shzxlz.cn

Ruby: exit 1
来源：http://htx.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kgh.havefunace.top

[M06] 向标准错误输出
来源：http://owu.bjfxy.top

Py:   print("err", file=sys.stderr)
来源：http://sox.zhijiandao.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vhm.hnxiangtu.top

JS:   console.error("err")
来源：http://jip.epnwcf.com

TS:   console.error("err")
来源：http://zko.chenlongwang.top

Java: System.err.println("err")
来源：http://akx.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://exv.cashguo.top

Ruby: warn "err"
来源：http://ehu.tarul.cn

C#:   Console.Error.WriteLine("err")
来源：http://xib.guannengcc.top

[M07] 判断是否为主入口
来源：http://abu.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://fmt.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jru.ehwqpu.com

JS:   require.main === module
来源：http://mwy.yangfankeji.com

TS:   require.main === module
来源：http://fcn.andypj.xyz

Java: public static void main(String[] args)
来源：http://ezg.hammf.cn

Go:   func main()
来源：http://ywq.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rui.yj202588.top

C#:   static void Main(string[] args)
来源：http://gjz.sweek.top

[M08] 获取系统与运行时信息
来源：http://jli.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://fgq.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://xfy.guannengcc.top

JS:   process.platform;  process.version
来源：http://bpb.zhengqikj.top

TS:   process.platform;  process.version
来源：http://nju.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://buk.uphjek.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://qyj.hnxiangtu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mzk.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vms.cashguo.top

================================================================================
来源：http://pdh.zdqjudy.top

N. 数据结构与算法
来源：http://nww.gzhubu.top

================================================================================
来源：http://kwg.sjlbkw.cn

[N01] 二分查找（有序数组）
来源：http://fdd.gogol.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nll.sxryk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ngx.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rma.shzxlz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wni.dianchejie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vtd.0kj1m.cn

Go:   sort.SearchInts(arr, x)
来源：http://rlv.svipenyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hlr.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://alq.hesvh.cn

[N02] 排序（工程实践用内置实现）
来源：http://jqb.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://sva.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iak.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://eki.cucudq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gzy.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mxd.ydzc1.top

Go:   slices.Sort(arr)
来源：http://htx.yj20258888.top

Ruby: arr.sort
来源：http://fcg.zdbjq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tlj.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://dnk.jinqigufen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ytt.redwolf501.top


<!-- 参考信息 -->