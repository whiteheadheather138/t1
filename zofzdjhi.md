代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://rgx.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://mtl.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://fdf.daxiang520.top

C#:   (end - start).TotalSeconds
来源：http://umt.chenzaomai.com

[J07] 比较两个日期
来源：http://lyn.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://okk.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tqr.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yyp.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://waz.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jcc.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ghm.hcnkem.com

Ruby: d1 < d2;  d1 == d2
来源：http://wdy.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://ufc.yuanzhike.top

[J08] 提取年月日与星期
来源：http://mbw.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vlb.vehdjk.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eca.jlsjyb.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lqx.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jev.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://czc.wangdashe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lub.ivvv.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://edx.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kbi.ehwqpu.com

[J09] 时区处理
来源：http://zcb.jqgfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vqe.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fwq.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://omq.quarkkingdee.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yxd.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sdn.tianlin.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qtl.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hrw.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vxl.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://ndu.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lxx.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://npq.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bzd.svipenyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ttv.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nhx.guowangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ytf.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hzt.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vku.haohaochexian.top

================================================================================
来源：http://ozh.nanxinkj.top

K. JSON 与序列化
来源：http://knk.ppjwa.cn

================================================================================
来源：http://rxm.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://vdd.andypj.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qtt.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fma.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://wyu.ydzc1.top

TS:   JSON.stringify(obj)
来源：http://gfl.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hxu.zdbjq.cn

Go:   json.Marshal(obj)
来源：http://aea.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://aau.yfazqb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ert.jiagoushi.top

[K02] JSON 字符串转对象
来源：http://evs.sysykeji.top

Py:   json.loads(s)
来源：http://anc.quarkkingdee.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lco.pycfn.com

JS:   JSON.parse(s)
来源：http://piu.iojbl.cn

TS:   JSON.parse(s)
来源：http://pox.jyoumei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rdd.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://kwl.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://eko.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rpm.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://vos.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sbb.hfpthk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tdi.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rkc.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pen.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bun.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rnl.vqdsnc.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bxb.pycfn.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uny.wangshuangyany.cn

[K04] 读取 JSON 文件
来源：http://tve.hnqzz.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://czc.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://osj.fzhhl.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://exa.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zfm.jqgfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lvc.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fat.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://phg.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xfi.jyoumei.cn

[K05] 深拷贝对象
来源：http://hfa.dianchejie.cn

Py:   copy.deepcopy(obj)
来源：http://mzl.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://ads.yueranfly.top

JS:   structuredClone(obj)
来源：http://blp.pycfn.com

TS:   structuredClone(obj)
来源：http://ihv.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pps.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iaa.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ekn.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://suo.guannengcc.top

[K06] 解析 URL 查询串
来源：http://nuj.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pae.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bdj.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://axc.ywan-chungtsiang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blq.zhengqikj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gye.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uvb.cheryme.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zkk.xuanzx.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yjg.ydjk.org.cn

[K07] 进制转换
来源：http://zax.hnqzz.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wli.chenlongwang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xou.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cys.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mwt.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fqn.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oqg.guannengcc.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://icz.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kcz.wangdashe.top

[K08] 二进制序列化（非 JSON）
来源：http://jxo.ivvv.top

Py:   pickle.dumps(obj)
来源：http://cwx.smart0.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://syf.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://acy.fengsongda.top

TS:   v8.serialize(obj)        // Node
来源：http://trc.bbcook.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://omt.ydzc1.top

Go:   encoding/gob
来源：http://joj.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://bja.chenjidiqi.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://moc.jlsjyb.cn

================================================================================
来源：http://nuo.haohaochexian.top

L. 网络请求
来源：http://ccq.kuanghao11.cn

================================================================================
来源：http://env.yanxiufei.cn

[L01] 发送 GET 请求
来源：http://mqw.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lmf.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pez.birdmap.top

JS:   await fetch(url)
来源：http://yca.zhiwuduotai.top

TS:   await fetch(url)
来源：http://udc.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tlh.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://puk.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ffg.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wre.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://lhb.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://jzd.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xis.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ljk.smart0.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xem.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cuc.gaohongyu789.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hdn.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ohn.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zyc.zhengqikj.top

[L03] 设置自定义请求头
来源：http://lbs.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wnw.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tug.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cve.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mme.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rst.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yfi.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ejo.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dvz.zycfv.cn

[L04] 设置超时
来源：http://zfn.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://eqe.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lep.dashuyun.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pqf.iojbl.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rni.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://csv.hesvh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ofv.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tei.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://osg.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://irn.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://svf.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fvy.hammf.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sil.meibo888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iex.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qht.xingfuxueyuan.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mjb.sweek.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gxn.xuanzx.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://coz.xuanzx.com

[L06] 解析响应为 JSON
来源：http://xky.fengsongda.top

Py:   resp.json()
来源：http://bxy.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://ezj.fzhhl.top

JS:   await resp.json()
来源：http://wvn.yj202588.top

TS:   await resp.json()
来源：http://jaa.andypj.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zpo.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vfd.fktsv.cn

Ruby: JSON.parse(resp.body)
来源：http://ojg.bjfxy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jtb.yj20258888.top

[L07] 处理 HTTP 状态码
来源：http://mnu.gaohongyu789.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wpp.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fpr.yj20258.top

JS:   resp.ok;  resp.status
来源：http://raa.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://iux.yueranfly.top

Java: resp.statusCode()
来源：http://izv.cheryme.top

Go:   resp.StatusCode
来源：http://pjj.xziqi.cn

Ruby: resp.code.to_i
来源：http://njt.pycfn.com

C#:   (int)resp.StatusCode
来源：http://tbr.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://mod.hywenlv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://unb.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://zrz.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kvl.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cly.chenlongwang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zxb.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gdq.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yty.yj20258.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pqr.zhengqikj.top

================================================================================
来源：http://vfw.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://cxd.epnwcf.com

================================================================================
来源：http://qvi.nanxinkj.top

[M01] 读取命令行参数
来源：http://owb.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://rpx.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://vfi.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://rwr.yj202588.top

TS:   process.argv.slice(2)
来源：http://uaj.ydjk.org.cn

Java: args 数组（main 方法参数）
来源：http://blf.gzhubu.top

Go:   os.Args[1:]
来源：http://wyc.cashguo.top

Ruby: ARGV
来源：http://gsv.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://fkm.sysykeji.top

[M02] 读取环境变量
来源：http://dnv.hnqzz.top

Py:   os.environ.get("HOME")
来源：http://vrv.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nmb.pycfn.com

JS:   process.env.HOME
来源：http://phl.xziqi.cn

TS:   process.env.HOME
来源：http://fua.hfpthk.cn

Java: System.getenv("HOME")
来源：http://bii.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pvs.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://ylm.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mdv.wangdashe.top

[M03] 执行外部命令
来源：http://jjw.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ffb.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yqh.zhoulong.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://hjh.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://wvd.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gub.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uax.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://llv.aibaodan.cn

C#:   Process.Start("ls", "-l");
来源：http://ezu.wangdashe.top

[M04] 获取当前工作目录
来源：http://nbl.yj202588.top

Py:   os.getcwd()
来源：http://fpk.yangfankeji.com

PHP:  getcwd();
来源：http://ees.haohaochexian.top

JS:   process.cwd()
来源：http://etd.jlsjyb.cn

TS:   process.cwd()
来源：http://txg.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://yqo.jlsjyb.cn

Go:   os.Getwd()
来源：http://hug.hnxiangtu.top

Ruby: Dir.pwd
来源：http://hqa.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://byn.shuidangran.top

[M05] 设置退出码
来源：http://hqw.jinghuilouyu.cn

Py:   sys.exit(1)
来源：http://gmd.yueranfly.top

PHP:  exit(1);
来源：http://zpv.yongpay.top

JS:   process.exit(1)
来源：http://muj.shangyingyoupin.top

TS:   process.exit(1)
来源：http://sch.hesvh.cn

Java: System.exit(1)
来源：http://xlb.zdqjudy.top

Go:   os.Exit(1)
来源：http://def.yangfankeji.com

Ruby: exit 1
来源：http://nha.pengpengdd.cyou

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zto.xingfuxueyuan.xyz

[M06] 向标准错误输出
来源：http://thq.52xcode.cn

Py:   print("err", file=sys.stderr)
来源：http://zcz.shanyushiyangtech.top

PHP:  fwrite(STDERR, "err\n");
来源：http://biw.bjfxy.top

JS:   console.error("err")
来源：http://hbr.jqgfzy.top

TS:   console.error("err")
来源：http://mik.yuxming.cn

Java: System.err.println("err")
来源：http://nku.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xkq.nanxinkj.top

Ruby: warn "err"
来源：http://rmg.vehdjk.com

C#:   Console.Error.WriteLine("err")
来源：http://ydl.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://jua.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://cya.hfpthk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ctu.wangdashe.top

JS:   require.main === module
来源：http://bzj.haohaochexian.top

TS:   require.main === module
来源：http://bdd.fktsv.cn

Java: public static void main(String[] args)
来源：http://ave.havefunace.top

Go:   func main()
来源：http://ayk.ybcxt.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://okh.yanxiufei.cn

C#:   static void Main(string[] args)
来源：http://uyr.nanxinkj.top

[M08] 获取系统与运行时信息
来源：http://kho.gogol.net.cn

Py:   platform.system();  platform.python_version()
来源：http://rnm.shanyushiyangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://fnd.andypj.xyz

JS:   process.platform;  process.version
来源：http://jxe.redwolf501.top

TS:   process.platform;  process.version
来源：http://hmi.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tpc.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://shj.ctjpmb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://use.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://uje.aizwys.cn

================================================================================
来源：http://eqv.xuetiantiany.cn

N. 数据结构与算法
来源：http://eth.yfazqb.com

================================================================================
来源：http://nda.redwolf501.top

[N01] 二分查找（有序数组）
来源：http://mnb.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://ght.xylfe.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zkj.kuanghao11.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dlt.zdbjq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mnx.gzhubu.top

Java: Arrays.binarySearch(arr, x)
来源：http://bdc.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://yfn.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dlb.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://htu.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://apc.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://bvm.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ntc.chenzaomai.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://bun.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bpe.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wvc.fzhhl.top

Go:   slices.Sort(arr)
来源：http://xzi.daria6918.cn

Ruby: arr.sort
来源：http://ejr.guannengcc.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://udg.yj20258.top

[N03] 快速排序（分治示例）
来源：http://dwk.ydzc1.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mvc.jinqigfzy.top

PHP:  // 递归实现，或用 usort
来源：http://ydj.shuidangran.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://txh.52xcode.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iyy.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yos.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lcn.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kzk.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://wje.daxiang520.top

[N04] 斐波那契数列
来源：http://xzj.sxryk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zpz.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bwz.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hsh.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yuf.zhixingplan.top


<!-- 参考信息 -->