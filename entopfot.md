代发 wailian999

Py:   (end - start).total_seconds()
来源：http://wos.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://lwa.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ttj.gzhubu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xpx.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xvn.shzxlz.cn

Go:   end.Sub(start).Hours()
来源：http://hmh.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://fgq.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://vqq.nanxinkj.top

[J07] 比较两个日期
来源：http://ums.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://vug.vehdjk.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wzk.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://wog.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://whn.gotoacloud.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gnm.uphjek.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vdt.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://cnm.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://dme.yonumen.top

[J08] 提取年月日与星期
来源：http://vnc.hongshengwenyu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zyr.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mcm.sysykeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ldw.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ftk.fzhhl.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ycz.chenjidiqi.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ypc.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fnx.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zpr.jqgfzy.top

[J09] 时区处理
来源：http://djf.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wbr.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://etv.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jch.zhijiandao.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rzw.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kda.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nmr.yueranfly.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fil.feifeiyinyue.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tbf.tian-w.cn

[J10] 取今天 / 本月第一天
来源：http://rol.smart0.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://ijs.fengsongda.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hfo.zhongyouzk.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ubh.shanyushiyangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://izi.yj20258.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ayo.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fef.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lsh.xingfuxueyuan.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://irc.jqgufenzy.top

================================================================================
来源：http://gmn.yangfankeji.com

K. JSON 与序列化
来源：http://kkl.wangdashe.top

================================================================================
来源：http://qtz.ehwqpu.com

[K01] 对象转 JSON 字符串
来源：http://dtv.zhoulong.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pni.daxiang520.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aqw.fzhhl.top

JS:   JSON.stringify(obj)
来源：http://rdl.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://bum.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pkw.andypj.xyz

Go:   json.Marshal(obj)
来源：http://msh.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dag.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lwk.xinyue.icu

[K02] JSON 字符串转对象
来源：http://wxk.hysaishi.cn

Py:   json.loads(s)
来源：http://bob.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zmv.ybcxt.top

JS:   JSON.parse(s)
来源：http://rao.aibaodan.cn

TS:   JSON.parse(s)
来源：http://qum.vqdsnc.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ssa.daxiang520.top

Go:   json.Unmarshal(data, &v)
来源：http://ccp.0kj1m.cn

Ruby: JSON.parse(s)
来源：http://tpr.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qsx.yueranfly.top

[K03] JSON 美化输出（带缩进）
来源：http://xvq.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jrj.cheryme.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wrf.cqqwz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jox.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bdn.jinqigfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xte.vqdsnc.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qwx.gotoacloud.top

Ruby: JSON.pretty_generate(obj)
来源：http://qum.hywenlv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://moq.yvedp.cn

[K04] 读取 JSON 文件
来源：http://pzt.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ofw.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hks.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zne.smart0.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kdp.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yxh.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rlo.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://amb.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zrh.meibo888.top

[K05] 深拷贝对象
来源：http://rfw.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://grg.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://whf.zhengqikj.top

JS:   structuredClone(obj)
来源：http://nzj.tarul.cn

TS:   structuredClone(obj)
来源：http://efr.zhongyouzk.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zpq.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xzu.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xhp.smart0.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://iii.tarul.cn

[K06] 解析 URL 查询串
来源：http://jbp.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://byx.cucudq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sao.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vad.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://avc.yonumen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gdp.xinyue.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://duw.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jkg.fehbvm.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cqf.xinyue.icu

[K07] 进制转换
来源：http://aqp.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jzh.hfpthk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jye.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://arn.cucudq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mri.jianghu66.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://agy.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ljj.yueranfly.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uno.yj202588.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://asp.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://ouy.tarul.cn

Py:   pickle.dumps(obj)
来源：http://avc.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rkz.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://iim.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://fmw.ywan-chungtsiang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pwt.tian-w.cn

Go:   encoding/gob
来源：http://zkx.guannengcc.top

Ruby: Marshal.dump(obj)
来源：http://lah.ybcxt.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mvr.zhixingplan.top

================================================================================
来源：http://aak.zhoulong.xyz

L. 网络请求
来源：http://scb.ctjpmb.com

================================================================================
来源：http://lox.hnqzz.top

[L01] 发送 GET 请求
来源：http://nqk.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://djq.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bqh.uphjek.com

JS:   await fetch(url)
来源：http://exn.nanxuanxn.top

TS:   await fetch(url)
来源：http://byp.ybcxt.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gvz.chenzaomai.com

Go:   resp, err := http.Get(url)
来源：http://ruv.sxryk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yhg.tian-w.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dfq.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://piu.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tri.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gjr.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://imj.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yhk.birdmap.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uag.xuanzx.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oek.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sex.uphjek.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lwg.ehwqpu.com

[L03] 设置自定义请求头
来源：http://maq.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gpy.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nnf.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pjf.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cbi.havefunace.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oml.jlsjyb.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vsw.shuidangran.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nil.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jnr.hnxiangtu.top

[L04] 设置超时
来源：http://rgx.zdqjudy.top

Py:   requests.get(url, timeout=5)
来源：http://elx.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nuj.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hfv.guannengcc.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://anx.aizwys.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rmt.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lmb.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nih.daria6918.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hsp.bbcook.cn

[L05] 上传文件（multipart）
来源：http://gmr.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bln.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fek.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://llg.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kbt.fanxiaobao.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zee.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zwz.wangshuangyany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://raa.dianchejie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nvn.shuidangran.top

[L06] 解析响应为 JSON
来源：http://iar.redwolf501.top

Py:   resp.json()
来源：http://pmx.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://opd.xylfe.cn

JS:   await resp.json()
来源：http://lpf.sjlbkw.cn

TS:   await resp.json()
来源：http://bac.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uyf.tian-w.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wkl.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://brx.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ibk.cashguo.top

[L07] 处理 HTTP 状态码
来源：http://qqv.iojbl.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://htu.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zpa.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://vdz.daxiang520.top

TS:   resp.ok;  resp.status
来源：http://cjr.hcnkem.com

Java: resp.statusCode()
来源：http://tbk.yongpay.top

Go:   resp.StatusCode
来源：http://lsx.wangdashe.top

Ruby: resp.code.to_i
来源：http://llf.pycfn.com

C#:   (int)resp.StatusCode
来源：http://vzq.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://npg.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jcq.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://diz.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bmb.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://trk.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fdg.jianghu66.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ktd.smart0.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cne.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nbg.ctjpmb.com

================================================================================
来源：http://npm.hnqzz.top

M. 命令行 / 进程 / 环境
来源：http://wlm.shanyushiyangtech.top

================================================================================
来源：http://znp.iojbl.cn

[M01] 读取命令行参数
来源：http://idx.9152youxi.cn

Py:   sys.argv[1:]
来源：http://ysv.zhengqikj.top

PHP:  $argv;  $argc;
来源：http://sjd.fanxiaobao.xyz

JS:   process.argv.slice(2)
来源：http://wgy.daria6918.cn

TS:   process.argv.slice(2)
来源：http://biv.ivvv.top

Java: args 数组（main 方法参数）
来源：http://crk.yanxiufei.cn

Go:   os.Args[1:]
来源：http://rti.uphjek.com

Ruby: ARGV
来源：http://gka.yonumen.top

C#:   args 数组（Main 方法参数）
来源：http://fjy.xziqi.cn

[M02] 读取环境变量
来源：http://ttf.tanke756.top

Py:   os.environ.get("HOME")
来源：http://xnk.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bws.fanxiaobao.xyz

JS:   process.env.HOME
来源：http://tne.yfazqb.com

TS:   process.env.HOME
来源：http://qvg.yangfankeji.com

Java: System.getenv("HOME")
来源：http://djc.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jwk.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://oyc.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aal.hammf.cn

[M03] 执行外部命令
来源：http://edy.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hao.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ulr.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://odw.yj202588.top

TS:   child_process.execSync("ls -l").toString()
来源：http://edz.bbcook.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vhf.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ejx.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uue.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://yhc.52xcode.cn

[M04] 获取当前工作目录
来源：http://grb.svipenyu.cn

Py:   os.getcwd()
来源：http://sch.haohaochexian.top

PHP:  getcwd();
来源：http://nel.fehbvm.com

JS:   process.cwd()
来源：http://bhy.ehwqpu.com

TS:   process.cwd()
来源：http://vhv.xylfe.cn

Java: Path.of("").toAbsolutePath()
来源：http://cek.nwbrower.top

Go:   os.Getwd()
来源：http://vpd.yj20258.top

Ruby: Dir.pwd
来源：http://rra.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://cmo.fengsongda.top

[M05] 设置退出码
来源：http://rea.dashuyun.cn

Py:   sys.exit(1)
来源：http://ogv.hongshengwenyu.top

PHP:  exit(1);
来源：http://ugd.chenzaomai.com

JS:   process.exit(1)
来源：http://gyz.gzhubu.top

TS:   process.exit(1)
来源：http://awd.zhengqikj.top

Java: System.exit(1)
来源：http://yli.yj202588.top

Go:   os.Exit(1)
来源：http://vkk.xylfe.cn

Ruby: exit 1
来源：http://uvf.ydjk.org.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://via.316326.xyz

[M06] 向标准错误输出
来源：http://oop.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://fqm.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rkx.hysaishi.cn

JS:   console.error("err")
来源：http://anz.daxiang520.top

TS:   console.error("err")
来源：http://cqp.birdmap.top

Java: System.err.println("err")
来源：http://vmj.zdqjudy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hac.tanke756.top

Ruby: warn "err"
来源：http://ezh.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://alr.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://zdd.svipenyu.cn

Py:   if __name__ == "__main__":
来源：http://xkw.ywan-chungtsiang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ttt.jiagoushi.top

JS:   require.main === module
来源：http://tjd.bjfxy.top

TS:   require.main === module
来源：http://pre.sweek.top

Java: public static void main(String[] args)
来源：http://ylq.cdnleiting.top

Go:   func main()
来源：http://xdo.gogol.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://snr.zhoulong.xyz

C#:   static void Main(string[] args)
来源：http://ofu.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://pug.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://yop.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://eoq.aibaodan.cn

JS:   process.platform;  process.version
来源：http://qyy.andypj.xyz

TS:   process.platform;  process.version
来源：http://buf.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pci.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mnu.hongshengwenyu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ztc.gaohongyu789.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qnd.c1oappe.top

================================================================================
来源：http://mnl.ehwqpu.com

N. 数据结构与算法
来源：http://bgz.zhijiandao.cn

================================================================================
来源：http://hcu.fzhhl.top

[N01] 二分查找（有序数组）
来源：http://ftx.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eza.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bbq.nanxinkj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mse.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xwt.shanyushiyangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://ego.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://sbx.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hoo.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://qlc.fktsv.cn

[N02] 排序（工程实践用内置实现）
来源：http://nuw.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://rgl.bbcook.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wzq.sxryk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hzp.hongshengwenyu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yum.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yqb.yonumen.top

Go:   slices.Sort(arr)
来源：http://xam.daxiang520.top

Ruby: arr.sort
来源：http://lxz.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bmi.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://wbh.shanyushiyangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bal.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://nrr.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ukd.xziqi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ugn.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hxl.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gxq.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wqj.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://mov.jinyuanbaomall.cn

[N04] 斐波那契数列
来源：http://ksf.sxryk.cn


<!-- 参考信息 -->