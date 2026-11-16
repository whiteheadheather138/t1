代发 wailian999

Py:   (end - start).total_seconds()
来源：http://pft.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://qzc.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gnv.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nre.cheryme.top

Java: Duration.between(start, end).toSeconds()
来源：http://kth.wangdashe.top

Go:   end.Sub(start).Hours()
来源：http://kmn.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://dup.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://kjk.jyoumei.cn

[J07] 比较两个日期
来源：http://tnl.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://puy.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://khu.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bip.xingfuxueyuan.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://jrp.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jng.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xif.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bri.yfazqb.com

C#:   d1 < d2;  d1 == d2
来源：http://ynd.nanxuanxn.top

[J08] 提取年月日与星期
来源：http://kap.hnqzz.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wio.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gvi.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ukg.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dga.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qvy.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://imr.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hoo.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uel.jqgufenzy.top

[J09] 时区处理
来源：http://sbh.daria6918.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ewn.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jaj.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pbl.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oik.jinyuanbaomall.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rds.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://san.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ksd.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ybr.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://gpd.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://icc.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sry.xuanzx.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ofp.yonumen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tqf.hysaishi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mpq.birdmap.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vgl.snrcjt.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iib.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ury.yanxiufei.cn

================================================================================
来源：http://ihl.zhijiandao.cn

K. JSON 与序列化
来源：http://lbh.jqgfzy.top

================================================================================
来源：http://xkd.guowangkeji.top

[K01] 对象转 JSON 字符串
来源：http://ead.fktsv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sow.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dxy.yuxming.cn

JS:   JSON.stringify(obj)
来源：http://wil.wangshuangyany.cn

TS:   JSON.stringify(obj)
来源：http://xic.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wax.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://kdx.hysaishi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wkm.shuidangran.top

C#:   JsonSerializer.Serialize(obj)
来源：http://guc.xinyue.icu

[K02] JSON 字符串转对象
来源：http://swv.zhiwuduotai.top

Py:   json.loads(s)
来源：http://nyb.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ykw.gotoacloud.top

JS:   JSON.parse(s)
来源：http://lnl.hywenlv.cn

TS:   JSON.parse(s)
来源：http://wem.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rfo.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://bnv.yongpay.top

Ruby: JSON.parse(s)
来源：http://ivb.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qdz.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://xsf.yuanzhike.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ujp.hysaishi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ajg.quarkkingdee.top

JS:   JSON.stringify(obj, null, 2)
来源：http://his.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://bre.hfpthk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://boa.smart0.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ozl.jqgfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://rua.dashuyun.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jkk.zhijiandao.cn

[K04] 读取 JSON 文件
来源：http://xnq.cucudq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://niy.fengsongda.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bfl.fanxiaobao.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fmh.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pea.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kbx.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kti.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lbb.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uci.snrcjt.cn

[K05] 深拷贝对象
来源：http://qgq.sysykeji.top

Py:   copy.deepcopy(obj)
来源：http://pqd.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://jza.sufxvd.cn

JS:   structuredClone(obj)
来源：http://qqj.jinqigfzy.top

TS:   structuredClone(obj)
来源：http://mpx.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wzl.ppjwa.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bbd.xuetiantiany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fzy.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dwo.jianghu66.top

[K06] 解析 URL 查询串
来源：http://tei.yanxiufei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oov.zdbjq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qoi.vqdsnc.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lzl.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eno.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jcx.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ghx.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nat.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dhs.uphjek.com

[K07] 进制转换
来源：http://qrr.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rlq.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ptk.316326.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://abe.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://epp.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xtb.aibaodan.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wuh.aizwys.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bwr.jinyuanbaomall.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lgv.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://pyj.ywan-chungtsiang.top

Py:   pickle.dumps(obj)
来源：http://zex.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://quf.tarul.cn

JS:   v8.serialize(obj)        // Node
来源：http://hwl.bbcook.cn

TS:   v8.serialize(obj)        // Node
来源：http://djs.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://guy.9152youxi.cn

Go:   encoding/gob
来源：http://rae.shzxlz.cn

Ruby: Marshal.dump(obj)
来源：http://jns.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xgo.chenzaomai.com

================================================================================
来源：http://jqv.jqgfzy.top

L. 网络请求
来源：http://ayn.9152youxi.cn

================================================================================
来源：http://ytc.xziqi.cn

[L01] 发送 GET 请求
来源：http://xwt.ivvv.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jga.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nok.ivvv.top

JS:   await fetch(url)
来源：http://aig.ctjpmb.com

TS:   await fetch(url)
来源：http://try.zdbjq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xol.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://gps.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://wiv.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aad.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://zvo.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://wep.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gjy.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vyn.hesvh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hpm.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uzj.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bsv.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lpf.hesvh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nbj.hnxiangtu.top

[L03] 设置自定义请求头
来源：http://jxg.mhx1999.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bhg.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ait.redwolf501.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://taz.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yps.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jxf.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zqp.vqdsnc.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gqu.jlsjyb.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wnr.jianghu66.top

[L04] 设置超时
来源：http://smi.hfpthk.cn

Py:   requests.get(url, timeout=5)
来源：http://raw.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zdz.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gwa.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qua.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zen.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dyi.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eun.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aln.yongpay.top

[L05] 上传文件（multipart）
来源：http://qfm.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://prq.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hzg.guannengcc.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jhq.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mpb.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wcp.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pan.sysykeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://saq.sxryk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uuu.c1oappe.top

[L06] 解析响应为 JSON
来源：http://cas.zdqjudy.top

Py:   resp.json()
来源：http://ark.ydzc1.top

PHP:  json_decode($body, true);
来源：http://vmr.ctjpmb.com

JS:   await resp.json()
来源：http://cxi.zhiwuduotai.top

TS:   await resp.json()
来源：http://qiv.hesvh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sbc.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wfg.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://txk.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kbq.tian-w.cn

[L07] 处理 HTTP 状态码
来源：http://pdn.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xmg.shanyushiyangtech.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lgg.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://klt.yuanzhike.top

TS:   resp.ok;  resp.status
来源：http://twv.zhaomingkeji.xyz

Java: resp.statusCode()
来源：http://aew.tarul.cn

Go:   resp.StatusCode
来源：http://zff.cashguo.top

Ruby: resp.code.to_i
来源：http://ufl.pengpengdd.cyou

C#:   (int)resp.StatusCode
来源：http://eig.quarkkingdee.top

[L08] 并发请求多个地址
来源：http://lio.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mky.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://noo.svipenyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uip.andypj.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gak.guowangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ldz.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gdk.uphjek.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yso.uphjek.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ydh.cashguo.top

================================================================================
来源：http://vrp.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://vqw.jlsjyb.cn

================================================================================
来源：http://hnn.zhongyouzk.top

[M01] 读取命令行参数
来源：http://mbb.xuanzx.com

Py:   sys.argv[1:]
来源：http://kbm.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://ebk.nwbrower.top

JS:   process.argv.slice(2)
来源：http://prw.hammf.cn

TS:   process.argv.slice(2)
来源：http://cny.daxiang520.top

Java: args 数组（main 方法参数）
来源：http://vxh.ydzc1.top

Go:   os.Args[1:]
来源：http://wlj.sweek.top

Ruby: ARGV
来源：http://wey.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://btc.hcnkem.com

[M02] 读取环境变量
来源：http://uyt.shuidangran.top

Py:   os.environ.get("HOME")
来源：http://hma.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jud.yongpay.top

JS:   process.env.HOME
来源：http://dhp.52xcode.cn

TS:   process.env.HOME
来源：http://cze.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://uem.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://obt.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://qib.hcnkem.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ofi.andypj.xyz

[M03] 执行外部命令
来源：http://pch.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://szu.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mcn.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://iil.hnxiangtu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://uet.fktsv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blz.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bhk.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://hqk.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://ffu.yonumen.top

[M04] 获取当前工作目录
来源：http://rwu.zycfv.cn

Py:   os.getcwd()
来源：http://rza.cdnleiting.top

PHP:  getcwd();
来源：http://rie.ppjwa.cn

JS:   process.cwd()
来源：http://oex.jlsjyb.cn

TS:   process.cwd()
来源：http://dpk.chenjidiqi.icu

Java: Path.of("").toAbsolutePath()
来源：http://oyz.yfazqb.com

Go:   os.Getwd()
来源：http://jwq.jinqigfzy.top

Ruby: Dir.pwd
来源：http://cmj.pycfn.com

C#:   Directory.GetCurrentDirectory()
来源：http://qxa.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://vwo.daxiang520.top

Py:   sys.exit(1)
来源：http://shw.meibo888.top

PHP:  exit(1);
来源：http://glk.sweek.top

JS:   process.exit(1)
来源：http://odm.chenzaomai.com

TS:   process.exit(1)
来源：http://pof.iojbl.cn

Java: System.exit(1)
来源：http://mci.sufxvd.cn

Go:   os.Exit(1)
来源：http://aag.quarkkingdee.top

Ruby: exit 1
来源：http://fvu.quarkkingdee.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jgd.shzxlz.cn

[M06] 向标准错误输出
来源：http://fnk.jlsjyb.cn

Py:   print("err", file=sys.stderr)
来源：http://ywh.cashguo.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fcr.snrcjt.cn

JS:   console.error("err")
来源：http://kzd.jqgfzy.top

TS:   console.error("err")
来源：http://tcu.xinyue.icu

Java: System.err.println("err")
来源：http://ftr.zhijiandao.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xzo.uphjek.com

Ruby: warn "err"
来源：http://zsf.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://svr.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://tjw.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://hvb.quarkkingdee.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://unj.dashuyun.cn

JS:   require.main === module
来源：http://aql.chenzaomai.com

TS:   require.main === module
来源：http://fds.zhengqikj.top

Java: public static void main(String[] args)
来源：http://vrs.yfazqb.com

Go:   func main()
来源：http://ohc.sufxvd.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dqx.jinqigfzy.top

C#:   static void Main(string[] args)
来源：http://skl.havefunace.top

[M08] 获取系统与运行时信息
来源：http://sww.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://rkt.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://lvd.xuanzx.com

JS:   process.platform;  process.version
来源：http://vkr.fzhhl.top

TS:   process.platform;  process.version
来源：http://ynr.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://khf.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zbn.wangshuangyany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tfj.jyoumei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bll.hywenlv.cn

================================================================================
来源：http://uak.yueranfly.top

N. 数据结构与算法
来源：http://jaq.daxiang520.top

================================================================================
来源：http://gvl.meibo888.top

[N01] 二分查找（有序数组）
来源：http://ake.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cjb.jianghu66.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rqe.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hop.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sva.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://oxc.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://gjl.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vhv.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://dfg.fengsongda.top

[N02] 排序（工程实践用内置实现）
来源：http://cjv.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://ddq.zdqjudy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nrw.birdmap.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zhe.hongshengwenyu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lxb.svipenyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jhm.gzhubu.top

Go:   slices.Sort(arr)
来源：http://hss.zycfv.cn

Ruby: arr.sort
来源：http://vsl.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://igx.gzhubu.top

[N03] 快速排序（分治示例）
来源：http://bwb.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dgr.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://fyy.jiagoushi.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uyz.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yxj.daria6918.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kjw.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dgn.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ofr.yanxiufei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vfo.yj20258888.top

[N04] 斐波那契数列
来源：http://soj.yfazqb.com


<!-- 参考信息 -->