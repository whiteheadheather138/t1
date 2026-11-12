代发 wailian999

[J07] 比较两个日期
来源：http://ovc.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://znb.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hjv.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cvd.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://zur.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kdm.zhijiandao.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eyc.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://tse.jqgufenzy.top

C#:   d1 < d2;  d1 == d2
来源：http://wpe.zdbjq.cn

[J08] 提取年月日与星期
来源：http://tub.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mja.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rmr.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mgb.yuanzhike.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gfl.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hsh.havefunace.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pwg.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jaf.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ysf.c1oappe.top

[J09] 时区处理
来源：http://dcs.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ylf.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ugk.hesvh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dqa.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lks.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mkn.fktsv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eau.gotoacloud.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fwy.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lvw.chenlongwang.top

[J10] 取今天 / 本月第一天
来源：http://qvd.hywenlv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bnv.epnwcf.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ple.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uex.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nul.cashguo.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sed.tian-w.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xzg.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nmq.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ggt.shangyingyoupin.top

================================================================================
来源：http://bqx.ydzc1.top

K. JSON 与序列化
来源：http://nje.cucudq.cn

================================================================================
来源：http://mwg.daria6918.cn

[K01] 对象转 JSON 字符串
来源：http://wpa.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qtu.tarul.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fnh.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://krb.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://ozz.andypj.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mlx.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://umc.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://myi.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zkl.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://rte.fanxiaobao.xyz

Py:   json.loads(s)
来源：http://oft.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jfs.daxiang520.top

JS:   JSON.parse(s)
来源：http://hrr.shanyushiyangtech.top

TS:   JSON.parse(s)
来源：http://bsa.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yrx.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://eko.52xcode.cn

Ruby: JSON.parse(s)
来源：http://jck.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ltg.daxiang520.top

[K03] JSON 美化输出（带缩进）
来源：http://dyg.svipenyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ujt.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ard.xuanzx.com

JS:   JSON.stringify(obj, null, 2)
来源：http://qeq.52xcode.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://edo.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://onm.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oxu.fktsv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zvi.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jbj.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://gjj.nanxuanxn.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tku.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cix.svipenyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tqp.jyoumei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ibg.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aqd.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zgj.hnxiangtu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ojb.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zps.snrcjt.cn

[K05] 深拷贝对象
来源：http://lpb.zhiwuduotai.top

Py:   copy.deepcopy(obj)
来源：http://hum.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://sak.zhengqikj.top

JS:   structuredClone(obj)
来源：http://lkf.tanke756.top

TS:   structuredClone(obj)
来源：http://bms.yueranfly.top

Java: // 手写拷贝构造，或序列化往返
来源：http://aja.yvedp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aeq.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cly.shangyingyoupin.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kvk.hfpthk.cn

[K06] 解析 URL 查询串
来源：http://ucf.kuanghao11.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sac.shuidangran.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wio.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wcq.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://reb.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ygr.zhaomingkeji.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://ofy.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://djq.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://feo.hysaishi.cn

[K07] 进制转换
来源：http://sjr.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bth.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rjn.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ssm.jinqigufen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yep.0kj1m.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fzf.sufxvd.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://efl.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rhf.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rcw.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://aiu.daria6918.cn

Py:   pickle.dumps(obj)
来源：http://isc.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://dmz.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://jrz.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://mjv.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://whp.yueranfly.top

Go:   encoding/gob
来源：http://dkn.tianlin.xyz

Ruby: Marshal.dump(obj)
来源：http://xts.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qyh.gotoacloud.top

================================================================================
来源：http://pku.yj20258.top

L. 网络请求
来源：http://ljk.vqdsnc.cn

================================================================================
来源：http://frj.hcnkem.com

[L01] 发送 GET 请求
来源：http://buh.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yze.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yhr.yuxming.cn

JS:   await fetch(url)
来源：http://vqi.bjfxy.top

TS:   await fetch(url)
来源：http://lfk.svipenyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fvi.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://zlw.gzhubu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yrg.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qkm.vehdjk.com

[L02] 发送 POST JSON
来源：http://gkz.jiagoushi.top

Py:   requests.post(url, json={"a": 1})
来源：http://qnd.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xex.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uuv.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://clc.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://phc.dianchejie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gax.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kqq.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jbj.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://oga.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tzg.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://atx.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://itu.hcnkem.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jbe.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dbr.jinqigfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ukl.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sxk.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wpj.tianlin.xyz

[L04] 设置超时
来源：http://vlu.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://znc.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bxg.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qth.yanxiufei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ugn.shangyingyoupin.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jdg.shanyushiyangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gvx.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sun.vehdjk.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mya.tianlin.xyz

[L05] 上传文件（multipart）
来源：http://vjn.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bor.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xyq.yuxming.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sxx.pengpengdd.cyou

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vqh.cdnleiting.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gwe.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bcw.smart0.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://viq.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gpa.gzhubu.top

[L06] 解析响应为 JSON
来源：http://pia.hfpthk.cn

Py:   resp.json()
来源：http://pxg.xinyue.icu

PHP:  json_decode($body, true);
来源：http://xax.hysaishi.cn

JS:   await resp.json()
来源：http://hxr.guannengcc.top

TS:   await resp.json()
来源：http://mwc.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wjq.jqgfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rse.shzxlz.cn

Ruby: JSON.parse(resp.body)
来源：http://ybw.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dqr.ywan-chungtsiang.top

[L07] 处理 HTTP 状态码
来源：http://sjd.yongpay.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mux.hongshengwenyu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fhi.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://trv.jiagoushi.top

TS:   resp.ok;  resp.status
来源：http://grk.snrcjt.cn

Java: resp.statusCode()
来源：http://uof.hnxiangtu.top

Go:   resp.StatusCode
来源：http://bhh.ctjpmb.com

Ruby: resp.code.to_i
来源：http://ulh.yj20258.top

C#:   (int)resp.StatusCode
来源：http://iyw.ppjwa.cn

[L08] 并发请求多个地址
来源：http://jju.ivvv.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kky.sysykeji.top

PHP:  curl_multi_init() 系列
来源：http://jae.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ofq.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mxq.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ptb.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cox.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kly.shanyushiyangtech.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ebt.hfpthk.cn

================================================================================
来源：http://udu.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://wek.birdmap.top

================================================================================
来源：http://ajz.epnwcf.com

[M01] 读取命令行参数
来源：http://fvg.bbcook.cn

Py:   sys.argv[1:]
来源：http://idv.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://efa.chenjidiqi.icu

JS:   process.argv.slice(2)
来源：http://rwi.nwbrower.top

TS:   process.argv.slice(2)
来源：http://cjj.zhijiandao.cn

Java: args 数组（main 方法参数）
来源：http://xnb.nwbrower.top

Go:   os.Args[1:]
来源：http://bii.jlsjyb.cn

Ruby: ARGV
来源：http://fon.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://lcy.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://cml.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://nss.hnqzz.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vdc.andypj.xyz

JS:   process.env.HOME
来源：http://ggh.316326.xyz

TS:   process.env.HOME
来源：http://uxp.chenzaomai.com

Java: System.getenv("HOME")
来源：http://hiv.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://puw.cashguo.top

Ruby: ENV["HOME"]
来源：http://ffh.kuanghao11.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pbh.ehwqpu.com

[M03] 执行外部命令
来源：http://tck.snrcjt.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mxr.svipenyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://puu.redwolf501.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ndf.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qyx.tarul.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bhg.chenzaomai.com

Go:   exec.Command("ls", "-l").Output()
来源：http://etd.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://kmn.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://gfp.cqqwz.cn

[M04] 获取当前工作目录
来源：http://spb.jqgfzy.top

Py:   os.getcwd()
来源：http://yte.jinghuilouyu.cn

PHP:  getcwd();
来源：http://dtd.xinyue.icu

JS:   process.cwd()
来源：http://urh.ivvv.top

TS:   process.cwd()
来源：http://gvt.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://txf.chenjidiqi.icu

Go:   os.Getwd()
来源：http://fqq.haohaochexian.top

Ruby: Dir.pwd
来源：http://frv.hywenlv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lpb.ybcxt.top

[M05] 设置退出码
来源：http://wjd.shuidangran.top

Py:   sys.exit(1)
来源：http://uon.epnwcf.com

PHP:  exit(1);
来源：http://lkc.redwolf501.top

JS:   process.exit(1)
来源：http://sri.smart0.xyz

TS:   process.exit(1)
来源：http://tpi.nanxinkj.top

Java: System.exit(1)
来源：http://ukf.ybcxt.top

Go:   os.Exit(1)
来源：http://uwl.xuanzx.com

Ruby: exit 1
来源：http://gaw.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://udi.vehdjk.com

[M06] 向标准错误输出
来源：http://cdw.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://whc.hongshengwenyu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uzk.jqgufenzy.top

JS:   console.error("err")
来源：http://doc.yongpay.top

TS:   console.error("err")
来源：http://ixh.haohaochexian.top

Java: System.err.println("err")
来源：http://cqb.yj20258888.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://png.gaohongyu789.top

Ruby: warn "err"
来源：http://bey.chenzaomai.com

C#:   Console.Error.WriteLine("err")
来源：http://gth.sweek.top

[M07] 判断是否为主入口
来源：http://jsv.meibo888.top

Py:   if __name__ == "__main__":
来源：http://rwj.xylfe.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qwb.316326.xyz

JS:   require.main === module
来源：http://wug.svipenyu.cn

TS:   require.main === module
来源：http://yfu.uphjek.com

Java: public static void main(String[] args)
来源：http://wml.yvedp.cn

Go:   func main()
来源：http://zzd.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rys.sxryk.cn

C#:   static void Main(string[] args)
来源：http://tjh.zhixingplan.top

[M08] 获取系统与运行时信息
来源：http://dxq.9152youxi.cn

Py:   platform.system();  platform.python_version()
来源：http://vpm.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://vfd.vehdjk.com

JS:   process.platform;  process.version
来源：http://knj.yj20258.top

TS:   process.platform;  process.version
来源：http://hma.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://urw.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://uen.zycfv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mcd.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cxq.tianlin.xyz

================================================================================
来源：http://dww.jlsjyb.cn

N. 数据结构与算法
来源：http://xwu.xylfe.cn

================================================================================
来源：http://dqs.zdbjq.cn

[N01] 二分查找（有序数组）
来源：http://jll.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dcy.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uzf.yanxiufei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iht.vehdjk.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rkr.svipenyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lvl.zhijiandao.cn

Go:   sort.SearchInts(arr, x)
来源：http://jct.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://keu.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://fux.xuanzx.com

[N02] 排序（工程实践用内置实现）
来源：http://sre.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://qua.hfpthk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fuw.vehdjk.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://woz.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://wfv.yanxiufei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hdz.hfpthk.cn

Go:   slices.Sort(arr)
来源：http://ipg.fengsongda.top

Ruby: arr.sort
来源：http://xdy.bjfxy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://oji.quarkkingdee.top

[N03] 快速排序（分治示例）
来源：http://tsj.haohaochexian.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mvd.fanxiaobao.xyz

PHP:  // 递归实现，或用 usort
来源：http://sjx.tanke756.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gbs.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ozk.sjlbkw.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ske.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://flm.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rlx.hesvh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pdh.wangshuangyany.cn

[N04] 斐波那契数列
来源：http://kzp.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vro.snrcjt.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jxf.ybcxt.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://afs.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lmx.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pdk.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cqu.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bzh.xylfe.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://als.tian-w.cn


<!-- 参考信息 -->