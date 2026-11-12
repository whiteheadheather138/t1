代发 wailian999

Py:   (end - start).total_seconds()
来源：http://nol.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://uvg.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eim.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iyx.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://qkm.aibaodan.cn

Go:   end.Sub(start).Hours()
来源：http://ony.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://bas.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://twq.9152youxi.cn

[J07] 比较两个日期
来源：http://ncz.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://bdp.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://weu.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tvh.nanxuanxn.top

TS:   d1.getTime() < d2.getTime()
来源：http://mni.yj20258888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xgk.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hfm.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mua.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://zvx.bjfxy.top

[J08] 提取年月日与星期
来源：http://lzr.ivvv.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nqm.yj20258.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nau.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xkh.uphjek.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kke.pengpengdd.cyou

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wkh.xinyue.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cmv.shangyingyoupin.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://afj.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xrv.jlsjyb.cn

[J09] 时区处理
来源：http://hue.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ycq.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://szt.wangdashe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gwh.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ggb.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cvq.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rkv.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yxn.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gfv.yangfankeji.com

[J10] 取今天 / 本月第一天
来源：http://cwy.shuidangran.top

Py:   date.today();  date.today().replace(day=1)
来源：http://sti.ppjwa.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://leu.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zsh.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ceb.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ozd.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bgw.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rno.sxryk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dzo.iojbl.cn

================================================================================
来源：http://xhp.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://rzu.zdqjudy.top

================================================================================
来源：http://ptx.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://pef.jlsjyb.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wkc.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tdz.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://muh.316326.xyz

TS:   JSON.stringify(obj)
来源：http://gut.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ghn.zhengqikj.top

Go:   json.Marshal(obj)
来源：http://woj.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://maz.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kyu.316326.xyz

[K02] JSON 字符串转对象
来源：http://lxj.dashuyun.cn

Py:   json.loads(s)
来源：http://pqk.nanxinkj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xiv.jqgfzy.top

JS:   JSON.parse(s)
来源：http://pda.jiagoushi.top

TS:   JSON.parse(s)
来源：http://uhm.jinqigufen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aeu.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://fes.cdnleiting.top

Ruby: JSON.parse(s)
来源：http://wij.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://asb.gzhubu.top

[K03] JSON 美化输出（带缩进）
来源：http://iet.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yaf.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fdz.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://stl.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ttc.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vhk.pycfn.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cqh.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://lfv.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ojx.nwbrower.top

[K04] 读取 JSON 文件
来源：http://dsr.hongshengwenyu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sly.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://crc.nanxinkj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uuh.zycfv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mds.shangyingyoupin.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hwt.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kmj.aibaodan.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://akl.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hri.uphjek.com

[K05] 深拷贝对象
来源：http://sgi.wangdashe.top

Py:   copy.deepcopy(obj)
来源：http://dzl.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://vzw.jqgfzy.top

JS:   structuredClone(obj)
来源：http://nga.birdmap.top

TS:   structuredClone(obj)
来源：http://rff.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mez.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uik.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rqd.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ooc.bbcook.cn

[K06] 解析 URL 查询串
来源：http://myo.kuanghao11.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dhs.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yho.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ion.sweek.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xfv.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://osk.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://klg.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sam.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dex.yangfankeji.com

[K07] 进制转换
来源：http://klu.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uer.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sfc.jinqigfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yyd.cucudq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jsm.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lbx.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wsa.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tyd.hfpthk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fuw.jinyuanbaomall.cn

[K08] 二进制序列化（非 JSON）
来源：http://yel.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://atg.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qqj.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://sks.hcnkem.com

TS:   v8.serialize(obj)        // Node
来源：http://bbu.fzhhl.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lde.gaohongyu789.top

Go:   encoding/gob
来源：http://eqs.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://vnv.tanke756.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cvk.xingfuxueyuan.xyz

================================================================================
来源：http://byp.jyoumei.cn

L. 网络请求
来源：http://nbn.cdnleiting.top

================================================================================
来源：http://dui.xinyue.icu

[L01] 发送 GET 请求
来源：http://qgt.ivvv.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://txr.birdmap.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pwx.jianghu66.top

JS:   await fetch(url)
来源：http://wug.nwbrower.top

TS:   await fetch(url)
来源：http://vwf.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hdf.zhongyouzk.top

Go:   resp, err := http.Get(url)
来源：http://hcq.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://ikk.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sur.yangfankeji.com

[L02] 发送 POST JSON
来源：http://ioe.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://mhp.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kyj.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bob.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lra.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uzt.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fmi.zycfv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fng.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bhu.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://azl.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dma.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zvs.yueranfly.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://enm.daria6918.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gzh.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rdv.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wws.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://axo.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aju.uphjek.com

[L04] 设置超时
来源：http://wyu.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://erl.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iih.0kj1m.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mcv.jiagoushi.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bcj.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://icf.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rri.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qtv.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kfy.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://gwc.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hmz.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iqw.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://spl.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uly.yonumen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://urj.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mei.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eyo.iojbl.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://umn.xylfe.cn

[L06] 解析响应为 JSON
来源：http://qrw.gzhubu.top

Py:   resp.json()
来源：http://pto.ppjwa.cn

PHP:  json_decode($body, true);
来源：http://cgn.xuetiantiany.cn

JS:   await resp.json()
来源：http://yet.quarkkingdee.top

TS:   await resp.json()
来源：http://xyy.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vlv.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mxz.xinyue.icu

Ruby: JSON.parse(resp.body)
来源：http://xpa.aibaodan.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xqw.shzxlz.cn

[L07] 处理 HTTP 状态码
来源：http://ahh.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://flh.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zzx.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://rww.xinyue.icu

TS:   resp.ok;  resp.status
来源：http://qag.52xcode.cn

Java: resp.statusCode()
来源：http://lav.vqdsnc.cn

Go:   resp.StatusCode
来源：http://pbh.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://khn.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://zdj.cheryme.top

[L08] 并发请求多个地址
来源：http://mna.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wvh.zhijiandao.cn

PHP:  curl_multi_init() 系列
来源：http://xsf.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zkd.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ntv.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eiz.xylfe.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kku.zhiwuduotai.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ceh.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mhd.shzxlz.cn

================================================================================
来源：http://zza.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://bti.feifeiyinyue.top

================================================================================
来源：http://wtu.fengsongda.top

[M01] 读取命令行参数
来源：http://lin.hnqzz.top

Py:   sys.argv[1:]
来源：http://abj.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://ahg.sxryk.cn

JS:   process.argv.slice(2)
来源：http://qjp.jinqigufen.top

TS:   process.argv.slice(2)
来源：http://lde.xziqi.cn

Java: args 数组（main 方法参数）
来源：http://dip.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://bzg.epnwcf.com

Ruby: ARGV
来源：http://frx.yj202588.top

C#:   args 数组（Main 方法参数）
来源：http://lip.hysaishi.cn

[M02] 读取环境变量
来源：http://isv.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://quk.haohaochexian.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ivc.zhijiandao.cn

JS:   process.env.HOME
来源：http://ebc.fktsv.cn

TS:   process.env.HOME
来源：http://cum.zhoulong.xyz

Java: System.getenv("HOME")
来源：http://zjr.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ssk.dianchejie.cn

Ruby: ENV["HOME"]
来源：http://tda.xinyue.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rae.birdmap.top

[M03] 执行外部命令
来源：http://ibs.guowangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lna.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cwx.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pcf.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://pzx.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eko.kuanghao11.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://asq.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qig.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://prv.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://qzw.hnqzz.top

Py:   os.getcwd()
来源：http://bvb.zhijiandao.cn

PHP:  getcwd();
来源：http://gdd.sjlbkw.cn

JS:   process.cwd()
来源：http://rli.guowangkeji.top

TS:   process.cwd()
来源：http://yav.zdbjq.cn

Java: Path.of("").toAbsolutePath()
来源：http://hrj.xuanzx.com

Go:   os.Getwd()
来源：http://iit.zhongyouzk.top

Ruby: Dir.pwd
来源：http://xzk.mhx1999.top

C#:   Directory.GetCurrentDirectory()
来源：http://zno.nanxinkj.top

[M05] 设置退出码
来源：http://xyy.chenlongwang.top

Py:   sys.exit(1)
来源：http://oha.vqdsnc.cn

PHP:  exit(1);
来源：http://fgz.hysaishi.cn

JS:   process.exit(1)
来源：http://azm.jiagoushi.top

TS:   process.exit(1)
来源：http://kra.shanyushiyangtech.top

Java: System.exit(1)
来源：http://ppa.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://etx.hfpthk.cn

Ruby: exit 1
来源：http://ajo.hnqzz.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ssw.nanxinkj.top

[M06] 向标准错误输出
来源：http://hrq.gotoacloud.top

Py:   print("err", file=sys.stderr)
来源：http://fpt.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://llg.c1oappe.top

JS:   console.error("err")
来源：http://pub.chenlongwang.top

TS:   console.error("err")
来源：http://oxk.yueranfly.top

Java: System.err.println("err")
来源：http://ity.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://slz.dianchejie.cn

Ruby: warn "err"
来源：http://pyi.haohaochexian.top

C#:   Console.Error.WriteLine("err")
来源：http://cfo.ywan-chungtsiang.top

[M07] 判断是否为主入口
来源：http://pib.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://xhb.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xkg.birdmap.top

JS:   require.main === module
来源：http://ggm.jinqigfzy.top

TS:   require.main === module
来源：http://urf.sufxvd.cn

Java: public static void main(String[] args)
来源：http://alk.ydjk.org.cn

Go:   func main()
来源：http://zhm.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nbq.shuidangran.top

C#:   static void Main(string[] args)
来源：http://odw.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://nee.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://ivi.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://twz.fktsv.cn

JS:   process.platform;  process.version
来源：http://mxx.tianlin.xyz

TS:   process.platform;  process.version
来源：http://bzv.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://prd.zycfv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dje.svipenyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yci.daria6918.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xfc.xziqi.cn

================================================================================
来源：http://lqi.cashguo.top

N. 数据结构与算法
来源：http://efz.yanxiufei.cn

================================================================================
来源：http://img.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://vej.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://isx.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eha.fzhhl.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wzt.ivvv.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uxu.sjlbkw.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vyj.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://xuo.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rjc.9152youxi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://udd.fktsv.cn

[N02] 排序（工程实践用内置实现）
来源：http://rdz.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://tbn.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nko.zhoulong.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://qhi.shangyingyoupin.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://enl.0kj1m.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qwg.xinyue.icu

Go:   slices.Sort(arr)
来源：http://nbm.yfazqb.com

Ruby: arr.sort
来源：http://jfg.ctjpmb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://jwg.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://dpg.yj20258888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://scz.tarul.cn

PHP:  // 递归实现，或用 usort
来源：http://hek.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hjy.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sls.hysaishi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://udd.yonumen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cmg.daria6918.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ltd.yonumen.top

C#:   // 手写递归，或 Array.Sort
来源：http://owt.nanxinkj.top

[N04] 斐波那契数列
来源：http://emk.yj20258.top


<!-- 参考信息 -->