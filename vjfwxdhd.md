代发 wailian999

[J07] 比较两个日期
来源：http://jiv.xuetiantiany.cn

Py:   d1 < d2;  d1 == d2
来源：http://nod.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dwy.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://ygv.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://mgg.dashuyun.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://owz.hcnkem.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bbz.ehwqpu.com

Ruby: d1 < d2;  d1 == d2
来源：http://bqn.jinqigufen.top

C#:   d1 < d2;  d1 == d2
来源：http://uis.vqdsnc.cn

[J08] 提取年月日与星期
来源：http://doq.dianchejie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://akc.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uzs.daxiang520.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://poz.zhaomingkeji.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pyu.c1oappe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://txr.yuanzhike.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gkj.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nnt.aibaodan.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xfe.jinghuilouyu.cn

[J09] 时区处理
来源：http://jat.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bfk.chenlongwang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fcy.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sbw.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jup.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vez.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bul.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://lqm.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nzq.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://nuf.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kwq.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bce.cqqwz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gli.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mrp.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bol.cashguo.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mbg.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ipz.redwolf501.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xem.ywan-chungtsiang.top

================================================================================
来源：http://rbo.chenlongwang.top

K. JSON 与序列化
来源：http://mie.daria6918.cn

================================================================================
来源：http://wdi.jlsjyb.cn

[K01] 对象转 JSON 字符串
来源：http://eny.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://brz.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://njp.yueranfly.top

JS:   JSON.stringify(obj)
来源：http://zyr.guowangkeji.top

TS:   JSON.stringify(obj)
来源：http://uzi.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yyf.guannengcc.top

Go:   json.Marshal(obj)
来源：http://wqa.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dqo.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qpx.jianghu66.top

[K02] JSON 字符串转对象
来源：http://nru.zdbjq.cn

Py:   json.loads(s)
来源：http://kgf.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ckz.shuidangran.top

JS:   JSON.parse(s)
来源：http://dto.xuanzx.com

TS:   JSON.parse(s)
来源：http://rnn.iojbl.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vjl.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://zsq.shanyushiyangkeji.top

Ruby: JSON.parse(s)
来源：http://kqt.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nqr.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://mto.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qil.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dir.birdmap.top

JS:   JSON.stringify(obj, null, 2)
来源：http://afn.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gtm.jqgufenzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://coo.cashguo.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bxk.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fvx.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aeg.xinyue.icu

[K04] 读取 JSON 文件
来源：http://epx.ivvv.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ubg.yj20258888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mjm.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://opp.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wta.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hjk.meibo888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wuv.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gos.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wjp.meibo888.top

[K05] 深拷贝对象
来源：http://byz.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://vzf.xuanzx.com

PHP:  unserialize(serialize($obj));
来源：http://dly.shuidangran.top

JS:   structuredClone(obj)
来源：http://zye.cdnleiting.top

TS:   structuredClone(obj)
来源：http://cov.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kqv.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dax.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://urq.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://zoc.shanyushiyangkeji.top

[K06] 解析 URL 查询串
来源：http://hah.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rsk.fzhhl.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fzw.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rfv.sysykeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sow.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nyt.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hmd.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://npo.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.redwolf501.top

[K07] 进制转换
来源：http://upv.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ojx.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wqu.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://spn.mhx1999.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rhe.cheryme.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cip.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mwu.ppjwa.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ajs.shangyingyoupin.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vlk.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://nef.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://dao.shanyushiyangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ejs.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://hag.mhx1999.top

TS:   v8.serialize(obj)        // Node
来源：http://ehs.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uyg.guannengcc.top

Go:   encoding/gob
来源：http://pwh.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://yaw.pycfn.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://slb.ydzc1.top

================================================================================
来源：http://tkl.xuanzx.com

L. 网络请求
来源：http://uwd.dianchejie.cn

================================================================================
来源：http://fem.ywan-chungtsiang.top

[L01] 发送 GET 请求
来源：http://rur.ydjk.org.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sba.yvedp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gbk.aizwys.cn

JS:   await fetch(url)
来源：http://tbx.hywenlv.cn

TS:   await fetch(url)
来源：http://hdb.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://toq.svipenyu.cn

Go:   resp, err := http.Get(url)
来源：http://dov.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://anb.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nvj.fktsv.cn

[L02] 发送 POST JSON
来源：http://tfn.birdmap.top

Py:   requests.post(url, json={"a": 1})
来源：http://njp.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cmj.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ejh.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bxd.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qhu.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ogt.guowangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rbv.chenjidiqi.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://erb.yonumen.top

[L03] 设置自定义请求头
来源：http://hng.hywenlv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fum.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://snh.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uab.hywenlv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qwa.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://chy.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hwi.hammf.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lrl.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://thj.hnxiangtu.top

[L04] 设置超时
来源：http://fnu.zhijiandao.cn

Py:   requests.get(url, timeout=5)
来源：http://ilv.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://adj.andypj.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rmy.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mrk.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mya.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wfa.fzhhl.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mfv.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tgf.sysykeji.top

[L05] 上传文件（multipart）
来源：http://wyt.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ozj.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kce.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bcj.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fll.316326.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hsc.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wtg.meibo888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kej.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ysr.nwbrower.top

[L06] 解析响应为 JSON
来源：http://ojl.feifeiyinyue.top

Py:   resp.json()
来源：http://vvq.xinyue.icu

PHP:  json_decode($body, true);
来源：http://zch.pycfn.com

JS:   await resp.json()
来源：http://ldg.yj202588.top

TS:   await resp.json()
来源：http://bts.zhengqikj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://faj.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://azr.pengpengdd.cyou

Ruby: JSON.parse(resp.body)
来源：http://eon.gaohongyu789.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zhl.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://oht.zhongyouzk.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hwg.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zpi.hammf.cn

JS:   resp.ok;  resp.status
来源：http://zri.yj20258.top

TS:   resp.ok;  resp.status
来源：http://tld.cashguo.top

Java: resp.statusCode()
来源：http://wkx.zdqjudy.top

Go:   resp.StatusCode
来源：http://bhi.dashuyun.cn

Ruby: resp.code.to_i
来源：http://cda.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://zmo.haohaochexian.top

[L08] 并发请求多个地址
来源：http://awq.tanke756.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://laf.shzxlz.cn

PHP:  curl_multi_init() 系列
来源：http://wjj.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rzx.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ore.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zpo.dianchejie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gve.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vnc.xziqi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hxc.yvedp.cn

================================================================================
来源：http://uyf.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://jbl.fehbvm.com

================================================================================
来源：http://fqt.hongshengwenyu.top

[M01] 读取命令行参数
来源：http://bni.jinqigfzy.top

Py:   sys.argv[1:]
来源：http://jwi.birdmap.top

PHP:  $argv;  $argc;
来源：http://hlk.gaohongyu789.top

JS:   process.argv.slice(2)
来源：http://zru.yonumen.top

TS:   process.argv.slice(2)
来源：http://yfc.xuanzx.com

Java: args 数组（main 方法参数）
来源：http://fuu.dianchejie.cn

Go:   os.Args[1:]
来源：http://dww.cucudq.cn

Ruby: ARGV
来源：http://obg.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://ytu.yonumen.top

[M02] 读取环境变量
来源：http://bfx.sjlbkw.cn

Py:   os.environ.get("HOME")
来源：http://iad.zhaomingkeji.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iwo.shangyingyoupin.top

JS:   process.env.HOME
来源：http://jcm.yfazqb.com

TS:   process.env.HOME
来源：http://ucs.cheryme.top

Java: System.getenv("HOME")
来源：http://ngl.gogol.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://irb.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://isl.c1oappe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tdf.shzxlz.cn

[M03] 执行外部命令
来源：http://xbp.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fpn.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ecd.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://umv.shangyingyoupin.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ubf.aibaodan.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xsw.fzhhl.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cnz.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vhr.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://rra.daria6918.cn

[M04] 获取当前工作目录
来源：http://mdj.sxryk.cn

Py:   os.getcwd()
来源：http://nif.cqqwz.cn

PHP:  getcwd();
来源：http://jsv.yuanzhike.top

JS:   process.cwd()
来源：http://ozl.shzxlz.cn

TS:   process.cwd()
来源：http://qhz.jqgufenzy.top

Java: Path.of("").toAbsolutePath()
来源：http://ecy.shangyingyoupin.top

Go:   os.Getwd()
来源：http://mke.jianghu66.top

Ruby: Dir.pwd
来源：http://zbd.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://ewn.fanxiaobao.xyz

[M05] 设置退出码
来源：http://ord.yonumen.top

Py:   sys.exit(1)
来源：http://acm.0kj1m.cn

PHP:  exit(1);
来源：http://nfx.wangdashe.top

JS:   process.exit(1)
来源：http://vou.jyoumei.cn

TS:   process.exit(1)
来源：http://wld.yangfankeji.com

Java: System.exit(1)
来源：http://exc.zycfv.cn

Go:   os.Exit(1)
来源：http://ywp.jyoumei.cn

Ruby: exit 1
来源：http://fye.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pen.dashuyun.cn

[M06] 向标准错误输出
来源：http://cbn.hysaishi.cn

Py:   print("err", file=sys.stderr)
来源：http://shz.xuetiantiany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qbp.bbcook.cn

JS:   console.error("err")
来源：http://inm.sweek.top

TS:   console.error("err")
来源：http://hum.uphjek.com

Java: System.err.println("err")
来源：http://ger.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ror.yonumen.top

Ruby: warn "err"
来源：http://acn.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://ica.daxiang520.top

[M07] 判断是否为主入口
来源：http://ntq.9152youxi.cn

Py:   if __name__ == "__main__":
来源：http://isr.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://prq.xylfe.cn

JS:   require.main === module
来源：http://sor.pycfn.com

TS:   require.main === module
来源：http://vax.birdmap.top

Java: public static void main(String[] args)
来源：http://xrn.hnqzz.top

Go:   func main()
来源：http://por.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yvm.shzxlz.cn

C#:   static void Main(string[] args)
来源：http://kng.pengpengdd.cyou

[M08] 获取系统与运行时信息
来源：http://pkf.ybcxt.top

Py:   platform.system();  platform.python_version()
来源：http://kpr.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://lbt.cqqwz.cn

JS:   process.platform;  process.version
来源：http://cdw.andypj.xyz

TS:   process.platform;  process.version
来源：http://dpj.cucudq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ifn.yfazqb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://hap.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rjf.kuanghao11.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eqr.yueranfly.top

================================================================================
来源：http://wpt.ydzc1.top

N. 数据结构与算法
来源：http://ehk.yfazqb.com

================================================================================
来源：http://afw.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://xsw.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://bpv.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kfx.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://evn.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lhc.svipenyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://owl.jinghuilouyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://fur.jinyuanbaomall.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://otl.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://fmc.yfazqb.com

[N02] 排序（工程实践用内置实现）
来源：http://dex.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://omz.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mrq.kuanghao11.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nou.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hxj.hcnkem.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dxr.nwbrower.top

Go:   slices.Sort(arr)
来源：http://rvm.quarkkingdee.top

Ruby: arr.sort
来源：http://qdy.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fdg.pycfn.com

[N03] 快速排序（分治示例）
来源：http://woh.wangdashe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jpc.wangshuangyany.cn

PHP:  // 递归实现，或用 usort
来源：http://deg.sweek.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rry.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aub.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ept.dianchejie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://syc.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aat.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ivz.xingfuxueyuan.xyz

[N04] 斐波那契数列
来源：http://zpi.aizwys.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zjr.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mcv.hnxiangtu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vwm.hnqzz.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ybi.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://utp.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vpc.xziqi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dbi.yvedp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rhi.jinqigfzy.top


<!-- 参考信息 -->