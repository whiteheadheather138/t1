代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fjr.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dwh.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://cdy.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://ptn.shzxlz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ezg.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ovz.c1oappe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ojc.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://ido.fengsongda.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uma.xziqi.cn

Ruby: Time.now + 7 * 86400
来源：http://cay.wangshuangyany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cjs.9152youxi.cn

[J06] 计算两时间之差
来源：http://gff.xziqi.cn

Py:   (end - start).total_seconds()
来源：http://zyh.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://ruw.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://icr.yueranfly.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vow.yonumen.top

Java: Duration.between(start, end).toSeconds()
来源：http://dqr.bjfxy.top

Go:   end.Sub(start).Hours()
来源：http://ull.epnwcf.com

Ruby: end - start                 # 返回秒数
来源：http://bgr.fzhhl.top

C#:   (end - start).TotalSeconds
来源：http://zcp.zhoulong.xyz

[J07] 比较两个日期
来源：http://siu.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://dgp.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ftt.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cxp.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://dws.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://owk.chenlongwang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qpx.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://dgq.316326.xyz

C#:   d1 < d2;  d1 == d2
来源：http://sow.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://osh.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://led.tian-w.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yrv.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dot.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kds.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ehg.chenlongwang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://olq.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bvg.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kun.nwbrower.top

[J09] 时区处理
来源：http://rrw.hongshengwenyu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://htb.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mbf.hywenlv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hfn.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lzy.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iac.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cxk.hfpthk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://orm.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dtc.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://yim.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://meq.zdbjq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fkr.9152youxi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jqg.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://shl.yonumen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yvg.kuanghao11.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rco.vqdsnc.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lqj.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wvf.9152youxi.cn

================================================================================
来源：http://nos.316326.xyz

K. JSON 与序列化
来源：http://mcy.gzhubu.top

================================================================================
来源：http://ret.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://pkm.kuanghao11.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tvu.epnwcf.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yyb.uphjek.com

JS:   JSON.stringify(obj)
来源：http://boy.zdqjudy.top

TS:   JSON.stringify(obj)
来源：http://pug.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ygj.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://tvc.yj20258.top

Ruby: obj.to_json                                     // require "json"
来源：http://pfp.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://eyq.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://gkn.jiagoushi.top

Py:   json.loads(s)
来源：http://znc.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oxd.xinyue.icu

JS:   JSON.parse(s)
来源：http://rcv.yueranfly.top

TS:   JSON.parse(s)
来源：http://qgp.birdmap.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://myi.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://tup.yj20258.top

Ruby: JSON.parse(s)
来源：http://ilg.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jwl.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://lvr.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sux.tian-w.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ieo.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ghc.jqgufenzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yuw.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qlu.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dhi.ivvv.top

Ruby: JSON.pretty_generate(obj)
来源：http://jxb.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://upk.gogol.net.cn

[K04] 读取 JSON 文件
来源：http://hrp.daxiang520.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tzv.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oxn.ppjwa.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cez.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fef.zhixingplan.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rjc.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eju.yfazqb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://rzl.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xew.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://tdk.ydjk.org.cn

Py:   copy.deepcopy(obj)
来源：http://ygs.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://uuh.birdmap.top

JS:   structuredClone(obj)
来源：http://ppc.iojbl.cn

TS:   structuredClone(obj)
来源：http://kmw.316326.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://xix.jqgfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fxu.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qlg.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yro.tanke756.top

[K06] 解析 URL 查询串
来源：http://mbo.chenlongwang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ahr.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hkv.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://trt.tanke756.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xcs.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kka.gaohongyu789.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://elc.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wsp.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://caz.zdqjudy.top

[K07] 进制转换
来源：http://ydh.ybcxt.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ddj.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dhh.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bhc.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nak.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gmq.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ubg.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uis.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sjf.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://xav.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://mth.zhijiandao.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uhl.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://ted.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://jop.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rhb.daxiang520.top

Go:   encoding/gob
来源：http://eev.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://syp.gaohongyu789.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://igc.jinqigufen.top

================================================================================
来源：http://sao.wangdashe.top

L. 网络请求
来源：http://brk.xingfuxueyuan.xyz

================================================================================
来源：http://efx.daria6918.cn

[L01] 发送 GET 请求
来源：http://spc.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rxo.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://air.xylfe.cn

JS:   await fetch(url)
来源：http://dsj.ppjwa.cn

TS:   await fetch(url)
来源：http://vqz.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wow.yuxming.cn

Go:   resp, err := http.Get(url)
来源：http://mjs.yongpay.top

Ruby: Net::HTTP.get(URI(url))
来源：http://snb.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://frj.dashuyun.cn

[L02] 发送 POST JSON
来源：http://uvj.hammf.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jup.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ebc.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fmd.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wfy.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mqu.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zty.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kia.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tav.bbcook.cn

[L03] 设置自定义请求头
来源：http://gri.fengsongda.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lca.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ygq.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tiy.ivvv.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yeb.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hsl.sjlbkw.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rsa.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rhe.haohaochexian.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mcs.ctjpmb.com

[L04] 设置超时
来源：http://mhl.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://nit.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hdr.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ykq.yueranfly.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ytw.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uga.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yrp.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ovy.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mwi.shanyushiyangkeji.top

[L05] 上传文件（multipart）
来源：http://ejt.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bfp.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ezv.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pjq.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qrn.hammf.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tcm.ctjpmb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qoc.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kav.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pof.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://wjw.wangshuangyany.cn

Py:   resp.json()
来源：http://skq.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://zai.zdqjudy.top

JS:   await resp.json()
来源：http://cbn.c1oappe.top

TS:   await resp.json()
来源：http://ntj.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iel.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://avf.xuanzx.com

Ruby: JSON.parse(resp.body)
来源：http://cla.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eov.hfpthk.cn

[L07] 处理 HTTP 状态码
来源：http://dhs.ppjwa.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ave.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wsi.jinyuanbaomall.cn

JS:   resp.ok;  resp.status
来源：http://ubf.jinqigufen.top

TS:   resp.ok;  resp.status
来源：http://lzo.yj20258888.top

Java: resp.statusCode()
来源：http://hrh.uphjek.com

Go:   resp.StatusCode
来源：http://urp.fehbvm.com

Ruby: resp.code.to_i
来源：http://dqr.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://dzy.hcnkem.com

[L08] 并发请求多个地址
来源：http://ilu.tanke756.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tdf.havefunace.top

PHP:  curl_multi_init() 系列
来源：http://iir.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kpq.jinqigufen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://een.daria6918.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://njd.dianchejie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://feu.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://inm.52xcode.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eow.tian-w.cn

================================================================================
来源：http://tkf.jiagoushi.top

M. 命令行 / 进程 / 环境
来源：http://byd.hfpthk.cn

================================================================================
来源：http://cwt.ehwqpu.com

[M01] 读取命令行参数
来源：http://jro.dianchejie.cn

Py:   sys.argv[1:]
来源：http://zef.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://rtx.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://thg.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://gqx.gogol.net.cn

Java: args 数组（main 方法参数）
来源：http://hfa.sysykeji.top

Go:   os.Args[1:]
来源：http://xyd.ehwqpu.com

Ruby: ARGV
来源：http://pvc.fehbvm.com

C#:   args 数组（Main 方法参数）
来源：http://iyr.yongpay.top

[M02] 读取环境变量
来源：http://sdb.zdbjq.cn

Py:   os.environ.get("HOME")
来源：http://suq.xziqi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hsx.cheryme.top

JS:   process.env.HOME
来源：http://tge.yuxming.cn

TS:   process.env.HOME
来源：http://sdj.xinyue.icu

Java: System.getenv("HOME")
来源：http://dgb.andypj.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oms.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://umi.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cig.zdqjudy.top

[M03] 执行外部命令
来源：http://enq.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rmi.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://seq.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hhn.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ktp.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cyo.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://knt.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gcn.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://hwn.tianlin.xyz

[M04] 获取当前工作目录
来源：http://kpe.tanke756.top

Py:   os.getcwd()
来源：http://ngv.chenjidiqi.icu

PHP:  getcwd();
来源：http://nfg.yueranfly.top

JS:   process.cwd()
来源：http://ghm.pengpengdd.cyou

TS:   process.cwd()
来源：http://kvz.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://ibo.nanxuanxn.top

Go:   os.Getwd()
来源：http://otq.xuetiantiany.cn

Ruby: Dir.pwd
来源：http://vkz.316326.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://gkn.zhijiandao.cn

[M05] 设置退出码
来源：http://hui.0kj1m.cn

Py:   sys.exit(1)
来源：http://xgv.uphjek.com

PHP:  exit(1);
来源：http://wcd.yvedp.cn

JS:   process.exit(1)
来源：http://rdo.tanke756.top

TS:   process.exit(1)
来源：http://vsp.quarkkingdee.top

Java: System.exit(1)
来源：http://kpk.zhongyouzk.top

Go:   os.Exit(1)
来源：http://sbv.yj20258.top

Ruby: exit 1
来源：http://kkd.yuxming.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ksv.redwolf501.top

[M06] 向标准错误输出
来源：http://cux.gogol.net.cn

Py:   print("err", file=sys.stderr)
来源：http://bif.svipenyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kyx.daxiang520.top

JS:   console.error("err")
来源：http://auu.fengsongda.top

TS:   console.error("err")
来源：http://upj.cdnleiting.top

Java: System.err.println("err")
来源：http://uqx.sweek.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ipl.ctjpmb.com

Ruby: warn "err"
来源：http://cso.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://wpa.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://fup.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://mgm.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uiv.yongpay.top

JS:   require.main === module
来源：http://iax.daria6918.cn

TS:   require.main === module
来源：http://eed.quarkkingdee.top

Java: public static void main(String[] args)
来源：http://eth.xuetiantiany.cn

Go:   func main()
来源：http://awu.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fmy.zhongyouzk.top

C#:   static void Main(string[] args)
来源：http://swb.mhx1999.top

[M08] 获取系统与运行时信息
来源：http://pmi.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://jis.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://olm.sjlbkw.cn

JS:   process.platform;  process.version
来源：http://rgx.shuidangran.top

TS:   process.platform;  process.version
来源：http://cej.yj20258888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hyk.jyoumei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://owx.pycfn.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yaa.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qix.vqdsnc.cn

================================================================================
来源：http://jrb.shanyushiyangtech.top

N. 数据结构与算法
来源：http://ppu.pycfn.com

================================================================================
来源：http://sfh.zhoulong.xyz

[N01] 二分查找（有序数组）
来源：http://mej.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lrm.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tnu.yfazqb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://stt.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xdg.gogol.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hhv.ywan-chungtsiang.top

Go:   sort.SearchInts(arr, x)
来源：http://bof.zdqjudy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vzg.fanxiaobao.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://vio.hammf.cn

[N02] 排序（工程实践用内置实现）
来源：http://unx.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://pbe.pengpengdd.cyou

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oly.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mnw.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mhg.epnwcf.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ayx.pengpengdd.cyou

Go:   slices.Sort(arr)
来源：http://xxv.nanxinkj.top


<!-- 参考信息 -->