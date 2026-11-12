代发 wailian999

Py:   (end - start).total_seconds()
来源：http://icw.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://pyn.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wwb.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eja.daxiang520.top

Java: Duration.between(start, end).toSeconds()
来源：http://npc.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://aow.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://rks.jinqigfzy.top

C#:   (end - start).TotalSeconds
来源：http://qih.dianchejie.cn

[J07] 比较两个日期
来源：http://gzw.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://tut.xziqi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://omb.zdbjq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kvs.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://txy.jinyuanbaomall.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tus.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bus.zhiwuduotai.top

Ruby: d1 < d2;  d1 == d2
来源：http://zef.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://uzz.nanxuanxn.top

[J08] 提取年月日与星期
来源：http://bet.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bzd.hnqzz.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cwf.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lrv.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://smp.yvedp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ehc.hysaishi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dpt.cheryme.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qqd.sweek.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ckw.kuanghao11.cn

[J09] 时区处理
来源：http://mmt.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vxx.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bpd.jinqigfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://clb.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mlj.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://igo.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ibi.yuxming.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ocm.sjlbkw.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qrd.shzxlz.cn

[J10] 取今天 / 本月第一天
来源：http://cph.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://shp.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://maw.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hmq.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nwm.yongpay.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zvd.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://voe.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mva.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://egt.guannengcc.top

================================================================================
来源：http://odx.tian-w.cn

K. JSON 与序列化
来源：http://snv.yanxiufei.cn

================================================================================
来源：http://xzy.xuetiantiany.cn

[K01] 对象转 JSON 字符串
来源：http://xpe.zhoulong.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zmr.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bbs.shangyingyoupin.top

JS:   JSON.stringify(obj)
来源：http://lsa.zhoulong.xyz

TS:   JSON.stringify(obj)
来源：http://bmc.shanyushiyangtech.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ers.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://bqe.jinqigfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://plr.vehdjk.com

C#:   JsonSerializer.Serialize(obj)
来源：http://lcx.jyoumei.cn

[K02] JSON 字符串转对象
来源：http://oat.snrcjt.cn

Py:   json.loads(s)
来源：http://liq.sjlbkw.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rxd.jyoumei.cn

JS:   JSON.parse(s)
来源：http://agi.fengsongda.top

TS:   JSON.parse(s)
来源：http://pqm.aibaodan.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uvs.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://ngw.316326.xyz

Ruby: JSON.parse(s)
来源：http://mxz.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hds.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://bjd.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xsi.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qls.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dtq.yongpay.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jds.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hdy.bjfxy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ikm.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ohl.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://igb.yonumen.top

[K04] 读取 JSON 文件
来源：http://mtx.ppjwa.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bao.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qna.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ing.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://psg.yj20258.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ioy.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pdy.yj20258888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dnl.birdmap.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hqx.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://udv.sweek.top

Py:   copy.deepcopy(obj)
来源：http://oux.xingfuxueyuan.xyz

PHP:  unserialize(serialize($obj));
来源：http://evh.aizwys.cn

JS:   structuredClone(obj)
来源：http://lyh.shuidangran.top

TS:   structuredClone(obj)
来源：http://inf.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hjf.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jco.52xcode.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sbp.jqgufenzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://von.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://lwj.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aoq.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rhz.jlsjyb.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dlf.hnqzz.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eyl.haohaochexian.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uwf.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rcn.ivvv.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://emy.ydzc1.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zfd.jinqigfzy.top

[K07] 进制转换
来源：http://mas.shuidangran.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fec.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fec.hnxiangtu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hcj.zhiwuduotai.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wgl.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xfg.shzxlz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nzn.ehwqpu.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vhk.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tzg.shuidangran.top

[K08] 二进制序列化（非 JSON）
来源：http://cpo.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://hpu.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ziq.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://wdc.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://mfa.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ajq.zdqjudy.top

Go:   encoding/gob
来源：http://tjy.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://kiv.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://irg.uphjek.com

================================================================================
来源：http://afz.tarul.cn

L. 网络请求
来源：http://qsz.yongpay.top

================================================================================
来源：http://pei.gotoacloud.top

[L01] 发送 GET 请求
来源：http://bmj.tian-w.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fal.cashguo.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qir.xylfe.cn

JS:   await fetch(url)
来源：http://mla.cheryme.top

TS:   await fetch(url)
来源：http://ofa.yonumen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xrc.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://puy.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ocm.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ura.yj202588.top

[L02] 发送 POST JSON
来源：http://sak.bbcook.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lfz.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://csr.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cnu.yanxiufei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jhp.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yvc.xingfuxueyuan.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://doy.chenjidiqi.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qzz.shangyingyoupin.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://urn.cdnleiting.top

[L03] 设置自定义请求头
来源：http://xrc.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ims.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iwn.yangfankeji.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dzr.aizwys.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jfe.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://chz.yuxming.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iyl.shangyingyoupin.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xht.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://czr.jinqigfzy.top

[L04] 设置超时
来源：http://qjs.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://kgc.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rve.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mwg.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://grk.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uik.fzhhl.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://orl.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://flz.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://spt.fehbvm.com

[L05] 上传文件（multipart）
来源：http://bpm.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hei.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kmx.quarkkingdee.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ekg.shanyushiyangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xaw.fehbvm.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ogy.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mys.nanxuanxn.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vco.wangshuangyany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uvq.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://toc.zhengqikj.top

Py:   resp.json()
来源：http://bsg.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://iuw.yuxming.cn

JS:   await resp.json()
来源：http://axr.jqgufenzy.top

TS:   await resp.json()
来源：http://hwv.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nvw.cheryme.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jhx.316326.xyz

Ruby: JSON.parse(resp.body)
来源：http://qzw.shangyingyoupin.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tqp.wangshuangyany.cn

[L07] 处理 HTTP 状态码
来源：http://ijh.kuanghao11.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fcb.gzhubu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dhq.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://gcp.zycfv.cn

TS:   resp.ok;  resp.status
来源：http://dmc.chenlongwang.top

Java: resp.statusCode()
来源：http://wza.shzxlz.cn

Go:   resp.StatusCode
来源：http://lsz.9152youxi.cn

Ruby: resp.code.to_i
来源：http://uqu.yj202588.top

C#:   (int)resp.StatusCode
来源：http://web.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://zta.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vje.pengpengdd.cyou

PHP:  curl_multi_init() 系列
来源：http://wbl.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://obv.zhiwuduotai.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dfi.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oyp.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cbg.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ypj.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://had.zhongyouzk.top

================================================================================
来源：http://xuu.zdbjq.cn

M. 命令行 / 进程 / 环境
来源：http://lcd.yangfankeji.com

================================================================================
来源：http://hhw.9152youxi.cn

[M01] 读取命令行参数
来源：http://geg.gotoacloud.top

Py:   sys.argv[1:]
来源：http://izw.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://vbr.wangdashe.top

JS:   process.argv.slice(2)
来源：http://ncs.jlsjyb.cn

TS:   process.argv.slice(2)
来源：http://xsu.hnqzz.top

Java: args 数组（main 方法参数）
来源：http://iti.yuxming.cn

Go:   os.Args[1:]
来源：http://sjp.shuidangran.top

Ruby: ARGV
来源：http://qkh.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://cdc.sjlbkw.cn

[M02] 读取环境变量
来源：http://djx.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://dbe.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lrw.redwolf501.top

JS:   process.env.HOME
来源：http://laa.cheryme.top

TS:   process.env.HOME
来源：http://ada.uphjek.com

Java: System.getenv("HOME")
来源：http://aar.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wid.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://uwv.hammf.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tpt.redwolf501.top

[M03] 执行外部命令
来源：http://egp.aizwys.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fxr.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qrv.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mok.fktsv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://npr.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dpc.316326.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://tnd.nanxuanxn.top

Ruby: system("ls -l");  `ls -l`
来源：http://pdb.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://eor.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://tss.dashuyun.cn

Py:   os.getcwd()
来源：http://qaa.yj202588.top

PHP:  getcwd();
来源：http://hez.shangyingyoupin.top

JS:   process.cwd()
来源：http://inz.zhijiandao.cn

TS:   process.cwd()
来源：http://sdn.sweek.top

Java: Path.of("").toAbsolutePath()
来源：http://rcl.yonumen.top

Go:   os.Getwd()
来源：http://haf.meibo888.top

Ruby: Dir.pwd
来源：http://ftt.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://sbj.hcnkem.com

[M05] 设置退出码
来源：http://xvm.hysaishi.cn

Py:   sys.exit(1)
来源：http://ucl.hcnkem.com

PHP:  exit(1);
来源：http://sbj.hfpthk.cn

JS:   process.exit(1)
来源：http://ywl.sysykeji.top

TS:   process.exit(1)
来源：http://yzu.0kj1m.cn

Java: System.exit(1)
来源：http://bdq.yanxiufei.cn

Go:   os.Exit(1)
来源：http://ejh.fzhhl.top

Ruby: exit 1
来源：http://vhg.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sag.yfazqb.com

[M06] 向标准错误输出
来源：http://zdx.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://ugb.shangyingyoupin.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ggv.cdnleiting.top

JS:   console.error("err")
来源：http://zgg.fzhhl.top

TS:   console.error("err")
来源：http://cnu.sysykeji.top

Java: System.err.println("err")
来源：http://dir.xylfe.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vhi.gaohongyu789.top

Ruby: warn "err"
来源：http://jkw.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://ims.316326.xyz

[M07] 判断是否为主入口
来源：http://spg.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://qph.yvedp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pgz.ydjk.org.cn

JS:   require.main === module
来源：http://ldx.zhengqikj.top

TS:   require.main === module
来源：http://aoy.zycfv.cn

Java: public static void main(String[] args)
来源：http://bqe.fanxiaobao.xyz

Go:   func main()
来源：http://eyo.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://aig.zdbjq.cn

C#:   static void Main(string[] args)
来源：http://buu.ivvv.top

[M08] 获取系统与运行时信息
来源：http://nzl.aibaodan.cn

Py:   platform.system();  platform.python_version()
来源：http://ljm.yonumen.top

PHP:  PHP_OS;  phpversion();
来源：http://myh.chenlongwang.top

JS:   process.platform;  process.version
来源：http://ysc.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://qam.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ewe.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vbq.jqgufenzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jui.fengsongda.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hrz.xingfuxueyuan.xyz

================================================================================
来源：http://exi.redwolf501.top

N. 数据结构与算法
来源：http://pqb.chenzaomai.com

================================================================================
来源：http://qqb.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://yyh.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://dyx.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cgr.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vsy.shangyingyoupin.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://srl.yj20258.top

Java: Arrays.binarySearch(arr, x)
来源：http://wjc.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://jkh.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://lib.gaohongyu789.top

C#:   Array.BinarySearch(arr, x)
来源：http://iud.birdmap.top

[N02] 排序（工程实践用内置实现）
来源：http://igf.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://ghq.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://srd.sxryk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vuw.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://iuy.fktsv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cdq.gogol.net.cn

Go:   slices.Sort(arr)
来源：http://vpv.jiagoushi.top

Ruby: arr.sort
来源：http://xpd.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zrx.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://gwj.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://boh.aibaodan.cn

PHP:  // 递归实现，或用 usort
来源：http://vhb.zhengqikj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mbh.yj20258.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blg.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vka.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://omt.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://drx.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xrg.ehwqpu.com

[N04] 斐波那契数列
来源：http://aug.zdqjudy.top


<!-- 参考信息 -->