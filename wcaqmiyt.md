代发 wailian999

[J07] 比较两个日期
来源：http://khk.chenjidiqi.icu

Py:   d1 < d2;  d1 == d2
来源：http://vqk.dianchejie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eeg.zhaomingkeji.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://twd.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hxx.chenzaomai.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gnj.sjlbkw.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kxk.zycfv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xsz.yanxiufei.cn

C#:   d1 < d2;  d1 == d2
来源：http://yoc.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://gvs.ivvv.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rum.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cqk.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bvx.hcnkem.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xmx.shanyushiyangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ptf.jinqigfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zvs.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qkv.yuxming.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kel.ywan-chungtsiang.top

[J09] 时区处理
来源：http://gmr.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uok.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hob.tian-w.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mqs.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://avu.xziqi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dqp.fzhhl.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mrs.zhoulong.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://ycs.316326.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ucw.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://ifi.svipenyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ndw.jinqigufen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oyr.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eiw.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eoj.zhijiandao.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://egm.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bxt.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ggc.guannengcc.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tmz.yj202588.top

================================================================================
来源：http://sdv.hongshengwenyu.top

K. JSON 与序列化
来源：http://ilm.uphjek.com

================================================================================
来源：http://bab.jlsjyb.cn

[K01] 对象转 JSON 字符串
来源：http://vdj.ivvv.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mhe.xuanzx.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gay.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://zbw.pycfn.com

TS:   JSON.stringify(obj)
来源：http://sya.zycfv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ofb.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://pqf.ydzc1.top

Ruby: obj.to_json                                     // require "json"
来源：http://eak.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qky.zhijiandao.cn

[K02] JSON 字符串转对象
来源：http://ktv.jiagoushi.top

Py:   json.loads(s)
来源：http://xjm.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iov.tian-w.cn

JS:   JSON.parse(s)
来源：http://ufq.jinyuanbaomall.cn

TS:   JSON.parse(s)
来源：http://imz.iojbl.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ouy.yj202588.top

Go:   json.Unmarshal(data, &v)
来源：http://lxc.ybcxt.top

Ruby: JSON.parse(s)
来源：http://kjy.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://apl.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://ify.guowangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hug.snrcjt.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qds.shuidangran.top

JS:   JSON.stringify(obj, null, 2)
来源：http://olc.fehbvm.com

TS:   JSON.stringify(obj, null, 2)
来源：http://twi.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wua.pengpengdd.cyou

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iie.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://shd.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tpm.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://tob.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gzr.tian-w.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fqa.ydjk.org.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pmf.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wvx.yangfankeji.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oub.zdqjudy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vtw.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ojw.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sgy.jianghu66.top

[K05] 深拷贝对象
来源：http://pcv.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://gye.epnwcf.com

PHP:  unserialize(serialize($obj));
来源：http://voc.chenzaomai.com

JS:   structuredClone(obj)
来源：http://fgw.sxryk.cn

TS:   structuredClone(obj)
来源：http://ded.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cdr.havefunace.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wot.yfazqb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wda.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://oqm.316326.xyz

[K06] 解析 URL 查询串
来源：http://kvu.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nks.hysaishi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fri.yonumen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jqx.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pee.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jfr.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://hfq.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qpv.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xdb.ywan-chungtsiang.top

[K07] 进制转换
来源：http://dvo.jinqigfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oui.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vza.yongpay.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tkc.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vib.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sfu.zhaomingkeji.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eei.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wma.shzxlz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sls.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://lvx.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://uph.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nps.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://myw.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://iuj.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vbw.cheryme.top

Go:   encoding/gob
来源：http://mde.ybcxt.top

Ruby: Marshal.dump(obj)
来源：http://nwr.yfazqb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hyx.xinyue.icu

================================================================================
来源：http://zgj.sjlbkw.cn

L. 网络请求
来源：http://hia.hysaishi.cn

================================================================================
来源：http://luy.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://ecc.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nbw.sufxvd.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://okt.hfpthk.cn

JS:   await fetch(url)
来源：http://omn.yj20258.top

TS:   await fetch(url)
来源：http://pzl.tianlin.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ehj.yueranfly.top

Go:   resp, err := http.Get(url)
来源：http://qda.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fxp.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lnj.snrcjt.cn

[L02] 发送 POST JSON
来源：http://yhv.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://lxy.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://phy.fengsongda.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zij.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mkb.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gbc.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ppf.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gtd.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cyv.zhoulong.xyz

[L03] 设置自定义请求头
来源：http://ont.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yew.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nbl.yongpay.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hui.jianghu66.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jod.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://llo.zhaomingkeji.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://evs.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qce.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pdn.pycfn.com

[L04] 设置超时
来源：http://fxf.nanxuanxn.top

Py:   requests.get(url, timeout=5)
来源：http://hvn.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nji.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yqc.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gov.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kvn.yonumen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jlo.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mus.zhongyouzk.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lyn.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://bke.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fzv.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ckf.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gte.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://any.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wvh.52xcode.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dss.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uvn.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gou.yuxming.cn

[L06] 解析响应为 JSON
来源：http://mjd.yj20258888.top

Py:   resp.json()
来源：http://ery.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://lbh.yongpay.top

JS:   await resp.json()
来源：http://wqf.xuanzx.com

TS:   await resp.json()
来源：http://jik.zdbjq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rxz.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bvb.hcnkem.com

Ruby: JSON.parse(resp.body)
来源：http://lna.sufxvd.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hcb.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://cvu.zdbjq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ilp.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yir.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://ysd.shangyingyoupin.top

TS:   resp.ok;  resp.status
来源：http://klu.andypj.xyz

Java: resp.statusCode()
来源：http://lvp.jiagoushi.top

Go:   resp.StatusCode
来源：http://cwo.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://wax.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://bwt.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://csz.xziqi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yik.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://uzy.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gmf.hfpthk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ula.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mkh.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zrh.hnxiangtu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gvg.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wsr.9152youxi.cn

================================================================================
来源：http://zzk.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://nek.yfazqb.com

================================================================================
来源：http://hrl.yuxming.cn

[M01] 读取命令行参数
来源：http://ulu.yj20258.top

Py:   sys.argv[1:]
来源：http://ybj.guannengcc.top

PHP:  $argv;  $argc;
来源：http://ghr.yj20258.top

JS:   process.argv.slice(2)
来源：http://usx.nanxinkj.top

TS:   process.argv.slice(2)
来源：http://dqm.shuidangran.top

Java: args 数组（main 方法参数）
来源：http://cga.epnwcf.com

Go:   os.Args[1:]
来源：http://lhx.cdnleiting.top

Ruby: ARGV
来源：http://iom.redwolf501.top

C#:   args 数组（Main 方法参数）
来源：http://rim.zdbjq.cn

[M02] 读取环境变量
来源：http://vkk.zdbjq.cn

Py:   os.environ.get("HOME")
来源：http://izd.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wvg.yanxiufei.cn

JS:   process.env.HOME
来源：http://gwd.yangfankeji.com

TS:   process.env.HOME
来源：http://htg.yuanzhike.top

Java: System.getenv("HOME")
来源：http://juv.zhoulong.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tvf.havefunace.top

Ruby: ENV["HOME"]
来源：http://rqg.yj20258888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kex.pengpengdd.cyou

[M03] 执行外部命令
来源：http://uqv.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://geh.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cfv.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ily.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qlf.aibaodan.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ujq.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zxo.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://hpa.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://hmz.iojbl.cn

[M04] 获取当前工作目录
来源：http://ldu.ybcxt.top

Py:   os.getcwd()
来源：http://lmn.feifeiyinyue.top

PHP:  getcwd();
来源：http://ifs.hywenlv.cn

JS:   process.cwd()
来源：http://xap.ybcxt.top

TS:   process.cwd()
来源：http://fsz.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://cac.jianghu66.top

Go:   os.Getwd()
来源：http://toz.sxryk.cn

Ruby: Dir.pwd
来源：http://lnl.cashguo.top

C#:   Directory.GetCurrentDirectory()
来源：http://uis.shzxlz.cn

[M05] 设置退出码
来源：http://aps.hammf.cn

Py:   sys.exit(1)
来源：http://njm.hammf.cn

PHP:  exit(1);
来源：http://xij.zdbjq.cn

JS:   process.exit(1)
来源：http://plb.0kj1m.cn

TS:   process.exit(1)
来源：http://ejo.tian-w.cn

Java: System.exit(1)
来源：http://byt.yj20258888.top

Go:   os.Exit(1)
来源：http://fer.zdbjq.cn

Ruby: exit 1
来源：http://sqe.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nkp.chenlongwang.top

[M06] 向标准错误输出
来源：http://nzb.shangyingyoupin.top

Py:   print("err", file=sys.stderr)
来源：http://tol.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ykk.jinqigfzy.top

JS:   console.error("err")
来源：http://qoe.birdmap.top

TS:   console.error("err")
来源：http://ijl.sweek.top

Java: System.err.println("err")
来源：http://tfb.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xuz.feifeiyinyue.top

Ruby: warn "err"
来源：http://sxz.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://bmf.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://wtt.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://toh.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dtr.sjlbkw.cn

JS:   require.main === module
来源：http://ixj.zhaomingkeji.xyz

TS:   require.main === module
来源：http://run.jinqigufen.top

Java: public static void main(String[] args)
来源：http://lxk.hcnkem.com

Go:   func main()
来源：http://avl.iojbl.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ldx.hnqzz.top

C#:   static void Main(string[] args)
来源：http://jdz.cheryme.top

[M08] 获取系统与运行时信息
来源：http://qub.fktsv.cn

Py:   platform.system();  platform.python_version()
来源：http://xfz.yj20258.top

PHP:  PHP_OS;  phpversion();
来源：http://rzq.yuanzhike.top

JS:   process.platform;  process.version
来源：http://lom.cucudq.cn

TS:   process.platform;  process.version
来源：http://mtq.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mvy.chenzaomai.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://jvq.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ztl.vqdsnc.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xgw.zdbjq.cn

================================================================================
来源：http://dwk.daria6918.cn

N. 数据结构与算法
来源：http://lge.bjfxy.top

================================================================================
来源：http://qch.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://gxu.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gjp.wangdashe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fgo.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wts.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://osg.yj20258.top

Java: Arrays.binarySearch(arr, x)
来源：http://vuq.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://mqt.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ufh.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://cdv.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://foq.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://rlf.epnwcf.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sye.vehdjk.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://sjc.nwbrower.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ayr.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nib.guowangkeji.top

Go:   slices.Sort(arr)
来源：http://omw.daria6918.cn

Ruby: arr.sort
来源：http://wwz.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zad.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://bqo.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wbc.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://luw.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ddo.zhoulong.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lhz.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uuy.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nfn.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://roc.pengpengdd.cyou

C#:   // 手写递归，或 Array.Sort
来源：http://juk.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://mxj.redwolf501.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pwf.jinqigfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hqg.hnxiangtu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nlh.daria6918.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pcr.zhijiandao.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://enb.zhijiandao.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sbx.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zfd.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pyx.hcnkem.com


<!-- 参考信息 -->