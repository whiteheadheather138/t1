代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://htq.vehdjk.com

Go:   end.Sub(start).Hours()
来源：http://edw.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://wrg.xinyue.icu

C#:   (end - start).TotalSeconds
来源：http://ixy.tian-w.cn

[J07] 比较两个日期
来源：http://fbe.cashguo.top

Py:   d1 < d2;  d1 == d2
来源：http://gqh.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xfg.hnqzz.top

JS:   d1.getTime() < d2.getTime()
来源：http://cvh.tanke756.top

TS:   d1.getTime() < d2.getTime()
来源：http://hmk.52xcode.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://moo.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hkl.jinghuilouyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yhs.jianghu66.top

C#:   d1 < d2;  d1 == d2
来源：http://rav.guannengcc.top

[J08] 提取年月日与星期
来源：http://wfj.cqqwz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nzu.xylfe.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://din.52xcode.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ouz.wangshuangyany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gql.hysaishi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://txt.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rkg.fzhhl.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vch.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nmx.sxryk.cn

[J09] 时区处理
来源：http://dqm.sweek.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hqc.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uie.xingfuxueyuan.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vlx.havefunace.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ize.xuanzx.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nzh.hongshengwenyu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jub.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dam.chenjidiqi.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://soe.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://ipy.epnwcf.com

Py:   date.today();  date.today().replace(day=1)
来源：http://drm.wangdashe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kwi.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wpk.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jlo.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bpg.jqgfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tby.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hzh.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eyc.xziqi.cn

================================================================================
来源：http://nvc.pengpengdd.cyou

K. JSON 与序列化
来源：http://zuw.nanxuanxn.top

================================================================================
来源：http://spr.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://ntu.gogol.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gxl.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zpk.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://vvs.jqgfzy.top

TS:   JSON.stringify(obj)
来源：http://fej.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mfu.daxiang520.top

Go:   json.Marshal(obj)
来源：http://sss.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://zwq.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://swi.jinqigufen.top

[K02] JSON 字符串转对象
来源：http://uiw.ybcxt.top

Py:   json.loads(s)
来源：http://evk.ybcxt.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dwr.shangyingyoupin.top

JS:   JSON.parse(s)
来源：http://emc.xziqi.cn

TS:   JSON.parse(s)
来源：http://fui.ydjk.org.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oya.cheryme.top

Go:   json.Unmarshal(data, &v)
来源：http://tfx.sjlbkw.cn

Ruby: JSON.parse(s)
来源：http://yzl.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cez.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://kyu.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rpa.zdqjudy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dzt.shuidangran.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tzj.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lgb.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://avz.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ebu.xuanzx.com

Ruby: JSON.pretty_generate(obj)
来源：http://llv.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://obj.hysaishi.cn

[K04] 读取 JSON 文件
来源：http://xkj.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qbd.kuanghao11.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rzl.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hqe.9152youxi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vti.hesvh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://udc.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zaz.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://kko.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ytq.hesvh.cn

[K05] 深拷贝对象
来源：http://szi.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://zay.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://brq.shanyushiyangtech.top

JS:   structuredClone(obj)
来源：http://lkm.yueranfly.top

TS:   structuredClone(obj)
来源：http://xkd.xylfe.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dlq.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qgk.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nue.epnwcf.com

C#:   // 序列化往返，或自定义 Clone
来源：http://otb.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://hle.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kld.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rxa.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dzn.pengpengdd.cyou

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lbj.yj20258888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jtq.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://lgt.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hvq.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zhm.aibaodan.cn

[K07] 进制转换
来源：http://sao.yj20258888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ltj.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yru.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nfb.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mop.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yax.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://reb.ywan-chungtsiang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zfw.hesvh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rks.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://dlq.dianchejie.cn

Py:   pickle.dumps(obj)
来源：http://sqf.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://trg.vehdjk.com

JS:   v8.serialize(obj)        // Node
来源：http://cwj.haohaochexian.top

TS:   v8.serialize(obj)        // Node
来源：http://aoz.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iri.yj20258888.top

Go:   encoding/gob
来源：http://kwh.gaohongyu789.top

Ruby: Marshal.dump(obj)
来源：http://ufk.shanyushiyangtech.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://avh.smart0.xyz

================================================================================
来源：http://fgr.sweek.top

L. 网络请求
来源：http://efl.daria6918.cn

================================================================================
来源：http://cgo.daxiang520.top

[L01] 发送 GET 请求
来源：http://lqb.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://diz.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lka.xinyue.icu

JS:   await fetch(url)
来源：http://ekm.cqqwz.cn

TS:   await fetch(url)
来源：http://ucx.hammf.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kbb.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://ecx.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ztr.xinyue.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kor.zdbjq.cn

[L02] 发送 POST JSON
来源：http://xdk.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tol.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xqn.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://izz.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jnv.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cxu.daxiang520.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jer.sjlbkw.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xex.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uqj.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://nut.xuanzx.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gpr.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jmd.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gsc.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qij.birdmap.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sqy.yongpay.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uzh.chenzaomai.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oap.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tvq.yueranfly.top

[L04] 设置超时
来源：http://zbq.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://yzg.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kbx.wangshuangyany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vtx.c1oappe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ubd.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xoa.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sqj.fzhhl.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rae.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zdt.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://wny.yuanzhike.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oyv.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://res.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vnp.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bvn.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ixk.52xcode.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qeq.hesvh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jup.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gpy.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://qsq.ywan-chungtsiang.top

Py:   resp.json()
来源：http://ivd.fzhhl.top

PHP:  json_decode($body, true);
来源：http://uby.yfazqb.com

JS:   await resp.json()
来源：http://rmx.cdnleiting.top

TS:   await resp.json()
来源：http://uec.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gdz.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rgd.ydzc1.top

Ruby: JSON.parse(resp.body)
来源：http://mly.hnqzz.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yco.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://eyu.guowangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fno.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dqe.aizwys.cn

JS:   resp.ok;  resp.status
来源：http://rdl.yanxiufei.cn

TS:   resp.ok;  resp.status
来源：http://kzw.redwolf501.top

Java: resp.statusCode()
来源：http://wsb.hywenlv.cn

Go:   resp.StatusCode
来源：http://fgb.snrcjt.cn

Ruby: resp.code.to_i
来源：http://qcu.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://rmh.mhx1999.top

[L08] 并发请求多个地址
来源：http://kft.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kce.shuidangran.top

PHP:  curl_multi_init() 系列
来源：http://lfw.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jqp.aibaodan.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bsh.zhixingplan.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pyp.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fpt.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://chq.9152youxi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yyi.bbcook.cn

================================================================================
来源：http://uoy.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://nuc.gzhubu.top

================================================================================
来源：http://efd.jinqigfzy.top

[M01] 读取命令行参数
来源：http://bpw.ppjwa.cn

Py:   sys.argv[1:]
来源：http://fdx.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://bqz.ybcxt.top

JS:   process.argv.slice(2)
来源：http://ubl.haohaochexian.top

TS:   process.argv.slice(2)
来源：http://wfi.guannengcc.top

Java: args 数组（main 方法参数）
来源：http://ygy.sxryk.cn

Go:   os.Args[1:]
来源：http://voz.vqdsnc.cn

Ruby: ARGV
来源：http://isl.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://kpc.pengpengdd.cyou

[M02] 读取环境变量
来源：http://xgf.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://tvx.guowangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rhz.sjlbkw.cn

JS:   process.env.HOME
来源：http://wma.zhijiandao.cn

TS:   process.env.HOME
来源：http://pdm.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://xmp.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uya.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://unj.xuanzx.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ane.c1oappe.top

[M03] 执行外部命令
来源：http://xqw.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bmu.wangdashe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://edi.ivvv.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nlq.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://bzp.epnwcf.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qae.pengpengdd.cyou

Go:   exec.Command("ls", "-l").Output()
来源：http://uri.yueranfly.top

Ruby: system("ls -l");  `ls -l`
来源：http://xly.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://zpl.zdqjudy.top

[M04] 获取当前工作目录
来源：http://apu.aizwys.cn

Py:   os.getcwd()
来源：http://gag.jinqigufen.top

PHP:  getcwd();
来源：http://tui.sysykeji.top

JS:   process.cwd()
来源：http://wmx.zdbjq.cn

TS:   process.cwd()
来源：http://ukr.gogol.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://jyr.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://fqp.snrcjt.cn

Ruby: Dir.pwd
来源：http://pds.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://yex.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://xau.hnqzz.top

Py:   sys.exit(1)
来源：http://tmp.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://lji.xziqi.cn

JS:   process.exit(1)
来源：http://hvv.zhixingplan.top

TS:   process.exit(1)
来源：http://vxx.redwolf501.top

Java: System.exit(1)
来源：http://rjx.fehbvm.com

Go:   os.Exit(1)
来源：http://mjo.epnwcf.com

Ruby: exit 1
来源：http://udc.zhixingplan.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xxb.ydjk.org.cn

[M06] 向标准错误输出
来源：http://dbm.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://sig.tanke756.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lnp.gotoacloud.top

JS:   console.error("err")
来源：http://gdo.tianlin.xyz

TS:   console.error("err")
来源：http://sqp.zhijiandao.cn

Java: System.err.println("err")
来源：http://ioq.aibaodan.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tcq.fanxiaobao.xyz

Ruby: warn "err"
来源：http://vmu.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://xbe.yueranfly.top

[M07] 判断是否为主入口
来源：http://riu.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://mxz.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uqw.zhixingplan.top

JS:   require.main === module
来源：http://hev.fanxiaobao.xyz

TS:   require.main === module
来源：http://zrp.cucudq.cn

Java: public static void main(String[] args)
来源：http://pwm.shangyingyoupin.top

Go:   func main()
来源：http://jtn.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eds.guannengcc.top

C#:   static void Main(string[] args)
来源：http://cfm.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://kpa.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://lcr.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://kni.jianghu66.top

JS:   process.platform;  process.version
来源：http://dtc.yj20258.top

TS:   process.platform;  process.version
来源：http://opi.guannengcc.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://clh.zhoulong.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://pka.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uds.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bnj.feifeiyinyue.top

================================================================================
来源：http://aoq.shuidangran.top

N. 数据结构与算法
来源：http://ksg.yvedp.cn

================================================================================
来源：http://lit.hcnkem.com

[N01] 二分查找（有序数组）
来源：http://jrm.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://mdl.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bgu.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yoz.chenjidiqi.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zvt.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://ntr.pycfn.com

Go:   sort.SearchInts(arr, x)
来源：http://kmu.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://adh.yj20258888.top

C#:   Array.BinarySearch(arr, x)
来源：http://aiu.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://cyg.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://opl.fanxiaobao.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tzh.jianghu66.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dso.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://xyo.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rmj.zycfv.cn

Go:   slices.Sort(arr)
来源：http://kjt.sufxvd.cn

Ruby: arr.sort
来源：http://qlu.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wid.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://kfo.xylfe.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gdr.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://oeo.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cgj.sweek.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iko.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tib.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://edu.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cmj.316326.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://rpk.hnxiangtu.top

[N04] 斐波那契数列
来源：http://dhh.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qxk.xuetiantiany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wgn.chenjidiqi.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tri.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pca.ybcxt.top


<!-- 参考信息 -->