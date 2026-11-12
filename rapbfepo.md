代发 wailian999

[J07] 比较两个日期
来源：http://mgf.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://ozq.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xqd.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://ppk.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gzm.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yjd.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ghg.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://wfz.aizwys.cn

C#:   d1 < d2;  d1 == d2
来源：http://exv.xziqi.cn

[J08] 提取年月日与星期
来源：http://nmq.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ofa.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://frd.fehbvm.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bqj.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wth.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jpx.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qeb.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xfi.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fhh.vehdjk.com

[J09] 时区处理
来源：http://paq.aizwys.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rry.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oaz.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lsb.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wib.guowangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://muk.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iss.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eja.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bek.daxiang520.top

[J10] 取今天 / 本月第一天
来源：http://frj.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cug.havefunace.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vlr.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qpb.jinqigfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vkz.hesvh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vkf.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hyt.chenzaomai.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://buk.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zoa.fktsv.cn

================================================================================
来源：http://lrr.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://wwe.yj202588.top

================================================================================
来源：http://hof.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://dms.hesvh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://heg.xziqi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wuo.sjlbkw.cn

JS:   JSON.stringify(obj)
来源：http://xzc.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://cvb.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ipp.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://wyj.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jfy.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://jtp.yuanzhike.top

[K02] JSON 字符串转对象
来源：http://rzu.shzxlz.cn

Py:   json.loads(s)
来源：http://gqw.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pep.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://arq.quarkkingdee.top

TS:   JSON.parse(s)
来源：http://drv.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ifs.tian-w.cn

Go:   json.Unmarshal(data, &v)
来源：http://jjb.yuxming.cn

Ruby: JSON.parse(s)
来源：http://oki.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pnq.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://gci.guannengcc.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pha.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nsc.tian-w.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tmk.ywan-chungtsiang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zca.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ycp.jinghuilouyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gya.vehdjk.com

Ruby: JSON.pretty_generate(obj)
来源：http://mfx.xziqi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://erz.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://fpq.jlsjyb.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lpg.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kxb.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xhb.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://raz.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wmh.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ghi.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fhu.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vdc.chenzaomai.com

[K05] 深拷贝对象
来源：http://kvd.yongpay.top

Py:   copy.deepcopy(obj)
来源：http://qkm.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://rhl.hnqzz.top

JS:   structuredClone(obj)
来源：http://yms.redwolf501.top

TS:   structuredClone(obj)
来源：http://xlu.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iat.hnqzz.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://haz.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nkl.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ibi.tarul.cn

[K06] 解析 URL 查询串
来源：http://fqd.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hgx.fzhhl.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ouq.birdmap.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xfl.0kj1m.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iyr.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hzo.hysaishi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hti.hfpthk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gvx.aizwys.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ovr.tianlin.xyz

[K07] 进制转换
来源：http://led.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rvg.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vjm.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xws.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fqt.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ebt.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dgh.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mkh.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://brf.gaohongyu789.top

[K08] 二进制序列化（非 JSON）
来源：http://ico.zhiwuduotai.top

Py:   pickle.dumps(obj)
来源：http://kiy.jqgufenzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mxz.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://uxs.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://buh.yueranfly.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aid.xinyue.icu

Go:   encoding/gob
来源：http://pva.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://eoq.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ujd.jiagoushi.top

================================================================================
来源：http://nfv.sxryk.cn

L. 网络请求
来源：http://pdd.zhoulong.xyz

================================================================================
来源：http://uxd.cheryme.top

[L01] 发送 GET 请求
来源：http://mer.yuxming.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oir.jqgufenzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ldu.ydzc1.top

JS:   await fetch(url)
来源：http://pcy.havefunace.top

TS:   await fetch(url)
来源：http://ceu.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://goy.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://igv.daria6918.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ppf.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qai.cucudq.cn

[L02] 发送 POST JSON
来源：http://smb.aizwys.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ews.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lie.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xfb.aizwys.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tkc.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sqm.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gtu.sjlbkw.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jgy.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ele.yuanzhike.top

[L03] 设置自定义请求头
来源：http://wmj.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fey.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://brt.nanxinkj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tpb.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gky.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ldn.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uty.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pvw.xinyue.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://alq.jinyuanbaomall.cn

[L04] 设置超时
来源：http://kzg.yj20258888.top

Py:   requests.get(url, timeout=5)
来源：http://mqg.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kgn.hesvh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hmi.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ubr.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ilk.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rdw.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ptb.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wrf.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://fiq.aibaodan.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cgg.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ekc.zhoulong.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bik.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zel.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hbd.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eby.wangshuangyany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rcu.nanxuanxn.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bjc.ywan-chungtsiang.top

[L06] 解析响应为 JSON
来源：http://shd.cheryme.top

Py:   resp.json()
来源：http://uhi.ywan-chungtsiang.top

PHP:  json_decode($body, true);
来源：http://owk.hcnkem.com

JS:   await resp.json()
来源：http://ozv.tanke756.top

TS:   await resp.json()
来源：http://jwl.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fnq.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wob.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://fhm.pengpengdd.cyou

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nzp.jinghuilouyu.cn

[L07] 处理 HTTP 状态码
来源：http://cij.daria6918.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sgg.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oyo.tianlin.xyz

JS:   resp.ok;  resp.status
来源：http://mtp.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://cem.cdnleiting.top

Java: resp.statusCode()
来源：http://zon.hysaishi.cn

Go:   resp.StatusCode
来源：http://fnt.vehdjk.com

Ruby: resp.code.to_i
来源：http://zyg.zhaomingkeji.xyz

C#:   (int)resp.StatusCode
来源：http://vhn.jqgfzy.top

[L08] 并发请求多个地址
来源：http://kqn.zhoulong.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://atr.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://fsd.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://myc.chenlongwang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eyt.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eyh.zhaomingkeji.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vmg.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ddl.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://msk.52xcode.cn

================================================================================
来源：http://aiw.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://qgh.shuidangran.top

================================================================================
来源：http://krq.meibo888.top

[M01] 读取命令行参数
来源：http://abv.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://als.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://ldc.chenlongwang.top

JS:   process.argv.slice(2)
来源：http://lve.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://onw.daxiang520.top

Java: args 数组（main 方法参数）
来源：http://hpl.jiagoushi.top

Go:   os.Args[1:]
来源：http://ctj.ydzc1.top

Ruby: ARGV
来源：http://wcy.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://smg.cashguo.top

[M02] 读取环境变量
来源：http://utr.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://pzf.dashuyun.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zdp.shzxlz.cn

JS:   process.env.HOME
来源：http://xpc.kuanghao11.cn

TS:   process.env.HOME
来源：http://mxg.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://umo.havefunace.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fvu.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://pby.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pkk.hfpthk.cn

[M03] 执行外部命令
来源：http://vic.pycfn.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hcj.yonumen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ufl.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ept.havefunace.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gkh.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tyj.zhoulong.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://ryr.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://bsy.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://ozf.zhoulong.xyz

[M04] 获取当前工作目录
来源：http://whc.pengpengdd.cyou

Py:   os.getcwd()
来源：http://tuf.316326.xyz

PHP:  getcwd();
来源：http://ssf.fehbvm.com

JS:   process.cwd()
来源：http://rbr.daria6918.cn

TS:   process.cwd()
来源：http://rei.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://coj.nanxuanxn.top

Go:   os.Getwd()
来源：http://gqw.pycfn.com

Ruby: Dir.pwd
来源：http://iby.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://hze.xinyue.icu

[M05] 设置退出码
来源：http://pwu.316326.xyz

Py:   sys.exit(1)
来源：http://vzn.vqdsnc.cn

PHP:  exit(1);
来源：http://wkn.yj202588.top

JS:   process.exit(1)
来源：http://mvf.fktsv.cn

TS:   process.exit(1)
来源：http://vlg.yuanzhike.top

Java: System.exit(1)
来源：http://lda.zhengqikj.top

Go:   os.Exit(1)
来源：http://frk.ywan-chungtsiang.top

Ruby: exit 1
来源：http://efr.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ojd.yueranfly.top

[M06] 向标准错误输出
来源：http://tyv.ydjk.org.cn

Py:   print("err", file=sys.stderr)
来源：http://civ.zhoulong.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://jyv.jyoumei.cn

JS:   console.error("err")
来源：http://btl.jinyuanbaomall.cn

TS:   console.error("err")
来源：http://fka.daxiang520.top

Java: System.err.println("err")
来源：http://lnh.vehdjk.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://efd.dashuyun.cn

Ruby: warn "err"
来源：http://vgt.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://hif.hywenlv.cn

[M07] 判断是否为主入口
来源：http://uhg.yj20258888.top

Py:   if __name__ == "__main__":
来源：http://ogz.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dow.sufxvd.cn

JS:   require.main === module
来源：http://aro.fzhhl.top

TS:   require.main === module
来源：http://ajf.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://bpt.vehdjk.com

Go:   func main()
来源：http://dul.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kty.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://zgq.bjfxy.top

[M08] 获取系统与运行时信息
来源：http://vbe.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://jrk.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://php.xuanzx.com

JS:   process.platform;  process.version
来源：http://ecv.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://kfe.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qph.fktsv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fie.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://arc.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mdi.birdmap.top

================================================================================
来源：http://dol.daxiang520.top

N. 数据结构与算法
来源：http://wfc.tian-w.cn

================================================================================
来源：http://oqg.shanyushiyangkeji.top

[N01] 二分查找（有序数组）
来源：http://ucq.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://dof.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bwa.redwolf501.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lwx.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://obl.sjlbkw.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hat.zhijiandao.cn

Go:   sort.SearchInts(arr, x)
来源：http://xjo.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aiy.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://qnc.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://otc.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://tpx.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jfg.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://xjl.nanxinkj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zcq.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jcc.tanke756.top

Go:   slices.Sort(arr)
来源：http://wlu.dashuyun.cn

Ruby: arr.sort
来源：http://uen.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wyy.fzhhl.top

[N03] 快速排序（分治示例）
来源：http://xgd.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fan.pengpengdd.cyou

PHP:  // 递归实现，或用 usort
来源：http://pps.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://abb.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fxx.yfazqb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xgp.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cnn.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ybu.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ckz.ehwqpu.com

[N04] 斐波那契数列
来源：http://kdn.yueranfly.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ocf.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hrw.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sam.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zjc.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fad.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gjy.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ssl.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wtj.uphjek.com


<!-- 参考信息 -->