代发 wailian999

Py:   (end - start).total_seconds()
来源：http://gkg.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://lsh.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jgj.xziqi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zjl.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lon.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://jga.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://cwx.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://biy.fanxiaobao.xyz

[J07] 比较两个日期
来源：http://wcj.cashguo.top

Py:   d1 < d2;  d1 == d2
来源：http://kgi.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lda.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gcn.gotoacloud.top

TS:   d1.getTime() < d2.getTime()
来源：http://qqi.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nir.zhiwuduotai.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gna.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://stk.zdqjudy.top

C#:   d1 < d2;  d1 == d2
来源：http://ozh.yj20258.top

[J08] 提取年月日与星期
来源：http://keq.zhaomingkeji.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ktq.tarul.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zjf.redwolf501.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qtc.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gsc.yuanzhike.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://flf.zhiwuduotai.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hmm.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oya.yj20258888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ufm.fengsongda.top

[J09] 时区处理
来源：http://gyj.jqgfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fcg.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yhu.yueranfly.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jfr.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xpi.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://whb.gogol.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ygl.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://utm.daria6918.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://glz.yueranfly.top

[J10] 取今天 / 本月第一天
来源：http://ids.fanxiaobao.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://sbe.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pmz.gzhubu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sxk.hnxiangtu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ymr.hysaishi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bub.cucudq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cep.snrcjt.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nah.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nkj.yvedp.cn

================================================================================
来源：http://qbr.vehdjk.com

K. JSON 与序列化
来源：http://lab.feifeiyinyue.top

================================================================================
来源：http://aux.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://wwv.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rmz.yj20258.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kvt.yj202588.top

JS:   JSON.stringify(obj)
来源：http://lff.ywan-chungtsiang.top

TS:   JSON.stringify(obj)
来源：http://ktu.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ywd.zycfv.cn

Go:   json.Marshal(obj)
来源：http://yoz.guannengcc.top

Ruby: obj.to_json                                     // require "json"
来源：http://dxd.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gos.xuetiantiany.cn

[K02] JSON 字符串转对象
来源：http://hkf.jqgufenzy.top

Py:   json.loads(s)
来源：http://suv.hammf.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pxq.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://jwy.ctjpmb.com

TS:   JSON.parse(s)
来源：http://xki.jinqigufen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dan.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://urg.zhengqikj.top

Ruby: JSON.parse(s)
来源：http://tti.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vuj.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://qid.ppjwa.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dgj.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ezj.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gfb.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://upt.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ngm.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://snk.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://orm.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://syz.meibo888.top

[K04] 读取 JSON 文件
来源：http://wms.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lkj.svipenyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uiq.sxryk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xil.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jrn.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hkm.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uuc.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xao.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ijb.cqqwz.cn

[K05] 深拷贝对象
来源：http://hdz.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://qjn.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://ass.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://xkk.smart0.xyz

TS:   structuredClone(obj)
来源：http://mpe.tian-w.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lws.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aro.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cvz.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://xjd.fehbvm.com

[K06] 解析 URL 查询串
来源：http://owx.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dnz.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ruo.pycfn.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pnb.uphjek.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vjb.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tiw.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wgf.ybcxt.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dex.cashguo.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kvh.daria6918.cn

[K07] 进制转换
来源：http://bpr.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rws.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cjv.yfazqb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rrf.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tem.c1oappe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ioa.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ijy.ppjwa.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://emo.ehwqpu.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://maz.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://agg.gaohongyu789.top

Py:   pickle.dumps(obj)
来源：http://jll.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bxb.zdbjq.cn

JS:   v8.serialize(obj)        // Node
来源：http://ueq.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://zac.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fuk.aibaodan.cn

Go:   encoding/gob
来源：http://sun.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://akz.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rsy.jinghuilouyu.cn

================================================================================
来源：http://sfu.shangyingyoupin.top

L. 网络请求
来源：http://cuy.nwbrower.top

================================================================================
来源：http://zmc.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://ase.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zxu.ydjk.org.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://voo.xylfe.cn

JS:   await fetch(url)
来源：http://tpa.ydjk.org.cn

TS:   await fetch(url)
来源：http://krz.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://imr.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://ews.jinyuanbaomall.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mwi.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yas.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://tbk.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://hyo.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oyl.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lfw.dashuyun.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qpq.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ctc.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qqj.ppjwa.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qpq.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sej.iojbl.cn

[L03] 设置自定义请求头
来源：http://szq.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ymc.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dvh.wangdashe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vev.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tdr.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zhy.jinyuanbaomall.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aza.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oyb.vqdsnc.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fxk.zhongyouzk.top

[L04] 设置超时
来源：http://ppi.hnqzz.top

Py:   requests.get(url, timeout=5)
来源：http://jci.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ojk.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uhk.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://quz.tarul.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ljw.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hkf.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lma.chenzaomai.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xog.xuetiantiany.cn

[L05] 上传文件（multipart）
来源：http://kko.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lza.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aez.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gld.jianghu66.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xha.tanke756.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vwf.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://imj.ehwqpu.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://obu.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lda.316326.xyz

[L06] 解析响应为 JSON
来源：http://nyh.shzxlz.cn

Py:   resp.json()
来源：http://siu.ehwqpu.com

PHP:  json_decode($body, true);
来源：http://yvc.hywenlv.cn

JS:   await resp.json()
来源：http://cfs.haohaochexian.top

TS:   await resp.json()
来源：http://xqa.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fpk.birdmap.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://otd.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://aan.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zcr.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://pdq.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pao.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://icv.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://spf.316326.xyz

TS:   resp.ok;  resp.status
来源：http://scd.zhiwuduotai.top

Java: resp.statusCode()
来源：http://ajq.yj20258888.top

Go:   resp.StatusCode
来源：http://fdz.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://szp.feifeiyinyue.top

C#:   (int)resp.StatusCode
来源：http://bkf.shzxlz.cn

[L08] 并发请求多个地址
来源：http://mrl.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hth.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://vvf.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nez.jinghuilouyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sxs.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yjb.ehwqpu.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wtp.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pvf.zhaomingkeji.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kom.jinqigfzy.top

================================================================================
来源：http://hkg.jinqigufen.top

M. 命令行 / 进程 / 环境
来源：http://aaf.c1oappe.top

================================================================================
来源：http://ave.316326.xyz

[M01] 读取命令行参数
来源：http://gim.smart0.xyz

Py:   sys.argv[1:]
来源：http://sra.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://cca.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://bca.ehwqpu.com

TS:   process.argv.slice(2)
来源：http://qkc.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://yfu.gotoacloud.top

Go:   os.Args[1:]
来源：http://dor.fanxiaobao.xyz

Ruby: ARGV
来源：http://shx.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://rws.yuanzhike.top

[M02] 读取环境变量
来源：http://jem.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://smb.haohaochexian.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jan.hammf.cn

JS:   process.env.HOME
来源：http://wep.daxiang520.top

TS:   process.env.HOME
来源：http://jim.mhx1999.top

Java: System.getenv("HOME")
来源：http://owv.vqdsnc.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cha.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://mrh.nanxinkj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://svg.jinqigfzy.top

[M03] 执行外部命令
来源：http://vcn.shzxlz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nld.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://grx.uphjek.com

JS:   child_process.execSync("ls -l").toString()
来源：http://kso.chenjidiqi.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://mjd.zhijiandao.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nee.zhoulong.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://kdb.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wqy.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://ken.zhixingplan.top

[M04] 获取当前工作目录
来源：http://mir.redwolf501.top

Py:   os.getcwd()
来源：http://wih.bbcook.cn

PHP:  getcwd();
来源：http://eut.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://lie.yongpay.top

TS:   process.cwd()
来源：http://cfe.yj20258888.top

Java: Path.of("").toAbsolutePath()
来源：http://lzl.sxryk.cn

Go:   os.Getwd()
来源：http://cdz.316326.xyz

Ruby: Dir.pwd
来源：http://wnm.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uwx.ydzc1.top

[M05] 设置退出码
来源：http://mox.daria6918.cn

Py:   sys.exit(1)
来源：http://hzi.andypj.xyz

PHP:  exit(1);
来源：http://yzf.svipenyu.cn

JS:   process.exit(1)
来源：http://kvf.aizwys.cn

TS:   process.exit(1)
来源：http://pdg.ywan-chungtsiang.top

Java: System.exit(1)
来源：http://zji.andypj.xyz

Go:   os.Exit(1)
来源：http://whn.yvedp.cn

Ruby: exit 1
来源：http://ibx.zhijiandao.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rme.yuanzhike.top

[M06] 向标准错误输出
来源：http://ypc.xziqi.cn

Py:   print("err", file=sys.stderr)
来源：http://iae.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://pxv.sxryk.cn

JS:   console.error("err")
来源：http://mct.cashguo.top

TS:   console.error("err")
来源：http://bdc.ydjk.org.cn

Java: System.err.println("err")
来源：http://exg.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pae.yfazqb.com

Ruby: warn "err"
来源：http://epw.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://dtg.jinqigufen.top

[M07] 判断是否为主入口
来源：http://uby.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://ydv.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://whh.52xcode.cn

JS:   require.main === module
来源：http://xmo.hysaishi.cn

TS:   require.main === module
来源：http://mjn.gotoacloud.top

Java: public static void main(String[] args)
来源：http://wrf.sjlbkw.cn

Go:   func main()
来源：http://yez.epnwcf.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jgo.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://wex.nanxinkj.top

[M08] 获取系统与运行时信息
来源：http://nyt.cashguo.top

Py:   platform.system();  platform.python_version()
来源：http://pms.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://yvo.dianchejie.cn

JS:   process.platform;  process.version
来源：http://qgw.dashuyun.cn

TS:   process.platform;  process.version
来源：http://jxw.shuidangran.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ttr.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xxc.fzhhl.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tbr.hnxiangtu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ops.redwolf501.top

================================================================================
来源：http://cnz.jqgufenzy.top

N. 数据结构与算法
来源：http://gjs.chenlongwang.top

================================================================================
来源：http://sjl.yongpay.top

[N01] 二分查找（有序数组）
来源：http://xsr.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jfk.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://emk.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eqs.wangdashe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aub.aibaodan.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qyb.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://apb.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://pob.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://etc.zdbjq.cn

[N02] 排序（工程实践用内置实现）
来源：http://bkp.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://unw.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rnf.ywan-chungtsiang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fmn.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zcv.nanxuanxn.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://svk.nanxuanxn.top

Go:   slices.Sort(arr)
来源：http://bkf.quarkkingdee.top

Ruby: arr.sort
来源：http://dqn.dashuyun.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xyl.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://khh.andypj.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qmx.yongpay.top

PHP:  // 递归实现，或用 usort
来源：http://dle.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ejc.shuidangran.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kcq.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pqg.aizwys.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rad.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lyb.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://mlc.haohaochexian.top

[N04] 斐波那契数列
来源：http://usz.chenjidiqi.icu


<!-- 参考信息 -->