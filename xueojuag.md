代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://xcf.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://dsp.zhiwuduotai.top

Ruby: end - start                 # 返回秒数
来源：http://fcs.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://ujc.xuanzx.com

[J07] 比较两个日期
来源：http://cls.epnwcf.com

Py:   d1 < d2;  d1 == d2
来源：http://qpx.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://udj.vehdjk.com

JS:   d1.getTime() < d2.getTime()
来源：http://con.zhiwuduotai.top

TS:   d1.getTime() < d2.getTime()
来源：http://uac.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bpn.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ubn.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://lsl.c1oappe.top

C#:   d1 < d2;  d1 == d2
来源：http://cqi.yangfankeji.com

[J08] 提取年月日与星期
来源：http://xdy.quarkkingdee.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nyo.yanxiufei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hlc.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kmo.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://upg.yvedp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wyv.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zoy.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ptk.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dxn.yj20258888.top

[J09] 时区处理
来源：http://vcq.havefunace.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kcp.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ytw.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://coc.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gxv.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sny.yongpay.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://afg.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sqm.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nxo.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://doy.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fvc.nanxuanxn.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gbp.hysaishi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aik.hcnkem.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nbb.shanyushiyangtech.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hem.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xdd.cheryme.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hyh.shanyushiyangtech.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rpl.zhoulong.xyz

================================================================================
来源：http://uyx.pengpengdd.cyou

K. JSON 与序列化
来源：http://aum.yj20258.top

================================================================================
来源：http://kth.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://kfd.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uen.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://adz.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://fmh.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://fye.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mdo.xziqi.cn

Go:   json.Marshal(obj)
来源：http://zgu.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uqa.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pxi.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://hta.shuidangran.top

Py:   json.loads(s)
来源：http://jpi.shanyushiyangtech.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://psg.ydjk.org.cn

JS:   JSON.parse(s)
来源：http://ljl.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://phw.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cpc.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://wxm.yvedp.cn

Ruby: JSON.parse(s)
来源：http://phn.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://laa.yvedp.cn

[K03] JSON 美化输出（带缩进）
来源：http://cml.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://odl.sxryk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bdy.c1oappe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ari.andypj.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://uev.zhengqikj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fnj.dianchejie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tyk.yangfankeji.com

Ruby: JSON.pretty_generate(obj)
来源：http://tlm.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oer.vqdsnc.cn

[K04] 读取 JSON 文件
来源：http://qco.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ovs.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://beq.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hpy.c1oappe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vfo.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://skp.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wvq.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zlt.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mtw.yangfankeji.com

[K05] 深拷贝对象
来源：http://gqd.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://npm.yangfankeji.com

PHP:  unserialize(serialize($obj));
来源：http://hys.zhixingplan.top

JS:   structuredClone(obj)
来源：http://xdd.yj202588.top

TS:   structuredClone(obj)
来源：http://xfm.ydzc1.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yed.jinyuanbaomall.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://grl.zhoulong.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://txx.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://eid.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://nfm.nanxinkj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qju.svipenyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fmn.hcnkem.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vut.epnwcf.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://smb.zhoulong.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vhq.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rqg.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rgh.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pzs.sweek.top

[K07] 进制转换
来源：http://hqe.svipenyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pdq.shangyingyoupin.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fii.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://psm.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gka.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://akg.yj202588.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rue.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jxa.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://arc.wangshuangyany.cn

[K08] 二进制序列化（非 JSON）
来源：http://jap.jlsjyb.cn

Py:   pickle.dumps(obj)
来源：http://prf.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://blk.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://vuc.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://mmn.haohaochexian.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nnr.shangyingyoupin.top

Go:   encoding/gob
来源：http://cco.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://fva.yj20258.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cxb.wangdashe.top

================================================================================
来源：http://uik.ybcxt.top

L. 网络请求
来源：http://lhi.sweek.top

================================================================================
来源：http://ziq.pycfn.com

[L01] 发送 GET 请求
来源：http://sob.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://msm.hnqzz.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qwa.ctjpmb.com

JS:   await fetch(url)
来源：http://xeb.ybcxt.top

TS:   await fetch(url)
来源：http://zak.sxryk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ymh.zhiwuduotai.top

Go:   resp, err := http.Get(url)
来源：http://adp.hfpthk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jdt.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kyd.gzhubu.top

[L02] 发送 POST JSON
来源：http://kmn.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://giu.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ldh.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vha.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://avp.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://izz.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rcu.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mia.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ujh.yvedp.cn

[L03] 设置自定义请求头
来源：http://zwy.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eei.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jwl.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://znz.ydjk.org.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kdq.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dpz.ppjwa.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vaj.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sxz.smart0.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xfj.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://voi.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://rfu.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://owh.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bzd.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dll.xylfe.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vwa.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ybb.havefunace.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mhu.tianlin.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://siy.pycfn.com

[L05] 上传文件（multipart）
来源：http://xad.nanxinkj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://alv.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qpm.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zhz.sysykeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ywe.mhx1999.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ahj.vqdsnc.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ytv.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cso.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://syt.daria6918.cn

[L06] 解析响应为 JSON
来源：http://eqh.yongpay.top

Py:   resp.json()
来源：http://alu.yonumen.top

PHP:  json_decode($body, true);
来源：http://ymv.tian-w.cn

JS:   await resp.json()
来源：http://ybu.zhixingplan.top

TS:   await resp.json()
来源：http://fil.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oau.andypj.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://scd.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://inn.sjlbkw.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cyr.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://grv.gotoacloud.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uht.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wrf.zdbjq.cn

JS:   resp.ok;  resp.status
来源：http://pqx.pengpengdd.cyou

TS:   resp.ok;  resp.status
来源：http://ijf.tianlin.xyz

Java: resp.statusCode()
来源：http://wec.sufxvd.cn

Go:   resp.StatusCode
来源：http://qcw.uphjek.com

Ruby: resp.code.to_i
来源：http://beo.yanxiufei.cn

C#:   (int)resp.StatusCode
来源：http://rol.hongshengwenyu.top

[L08] 并发请求多个地址
来源：http://gzt.bbcook.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qgj.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://dtp.hnxiangtu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://emq.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rwj.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oad.zhaomingkeji.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://odg.cdnleiting.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sbz.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sgw.jinqigufen.top

================================================================================
来源：http://alx.hammf.cn

M. 命令行 / 进程 / 环境
来源：http://zze.snrcjt.cn

================================================================================
来源：http://weo.bbcook.cn

[M01] 读取命令行参数
来源：http://pan.shanyushiyangtech.top

Py:   sys.argv[1:]
来源：http://iyo.jinqigfzy.top

PHP:  $argv;  $argc;
来源：http://fni.quarkkingdee.top

JS:   process.argv.slice(2)
来源：http://zir.yvedp.cn

TS:   process.argv.slice(2)
来源：http://kyx.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://qte.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://qra.yonumen.top

Ruby: ARGV
来源：http://jlu.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://oos.316326.xyz

[M02] 读取环境变量
来源：http://ntq.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://hif.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ulw.iojbl.cn

JS:   process.env.HOME
来源：http://mqr.yuxming.cn

TS:   process.env.HOME
来源：http://faw.xuanzx.com

Java: System.getenv("HOME")
来源：http://azp.hesvh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ivi.uphjek.com

Ruby: ENV["HOME"]
来源：http://zqd.guannengcc.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wpz.nanxinkj.top

[M03] 执行外部命令
来源：http://fmc.svipenyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wpt.ydzc1.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qjk.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ynz.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fpp.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ave.kuanghao11.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tus.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://iqk.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://qha.fktsv.cn

[M04] 获取当前工作目录
来源：http://scz.redwolf501.top

Py:   os.getcwd()
来源：http://jxt.hesvh.cn

PHP:  getcwd();
来源：http://ovw.yuanzhike.top

JS:   process.cwd()
来源：http://ljs.epnwcf.com

TS:   process.cwd()
来源：http://dab.yueranfly.top

Java: Path.of("").toAbsolutePath()
来源：http://cet.ydzc1.top

Go:   os.Getwd()
来源：http://txc.jianghu66.top

Ruby: Dir.pwd
来源：http://bep.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://ptd.ydzc1.top

[M05] 设置退出码
来源：http://szj.tianlin.xyz

Py:   sys.exit(1)
来源：http://scz.fanxiaobao.xyz

PHP:  exit(1);
来源：http://vbk.sweek.top

JS:   process.exit(1)
来源：http://ypk.gogol.net.cn

TS:   process.exit(1)
来源：http://nbb.xziqi.cn

Java: System.exit(1)
来源：http://smx.yfazqb.com

Go:   os.Exit(1)
来源：http://hzs.zhoulong.xyz

Ruby: exit 1
来源：http://zhh.meibo888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tux.hcnkem.com

[M06] 向标准错误输出
来源：http://mfo.redwolf501.top

Py:   print("err", file=sys.stderr)
来源：http://rzc.pengpengdd.cyou

PHP:  fwrite(STDERR, "err\n");
来源：http://gta.yuxming.cn

JS:   console.error("err")
来源：http://xcq.yueranfly.top

TS:   console.error("err")
来源：http://olc.aibaodan.cn

Java: System.err.println("err")
来源：http://pce.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pdv.xinyue.icu

Ruby: warn "err"
来源：http://sox.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://jdv.fengsongda.top

[M07] 判断是否为主入口
来源：http://vsp.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://tib.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nwy.xingfuxueyuan.xyz

JS:   require.main === module
来源：http://uss.dianchejie.cn

TS:   require.main === module
来源：http://bon.jinghuilouyu.cn

Java: public static void main(String[] args)
来源：http://bac.yfazqb.com

Go:   func main()
来源：http://rzj.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jlx.svipenyu.cn

C#:   static void Main(string[] args)
来源：http://twz.quarkkingdee.top

[M08] 获取系统与运行时信息
来源：http://ccy.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://kfc.xingfuxueyuan.xyz

PHP:  PHP_OS;  phpversion();
来源：http://uyy.fehbvm.com

JS:   process.platform;  process.version
来源：http://liu.smart0.xyz

TS:   process.platform;  process.version
来源：http://sia.zdqjudy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://auy.havefunace.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fjb.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jcd.nanxinkj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tck.birdmap.top

================================================================================
来源：http://ggx.quarkkingdee.top

N. 数据结构与算法
来源：http://axk.snrcjt.cn

================================================================================
来源：http://uxt.sysykeji.top

[N01] 二分查找（有序数组）
来源：http://vvg.ivvv.top

Py:   bisect.bisect_left(arr, x)
来源：http://dsr.hesvh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xdn.feifeiyinyue.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gjg.dianchejie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zfg.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://czs.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://wcj.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gfv.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gdy.hfpthk.cn

[N02] 排序（工程实践用内置实现）
来源：http://vho.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://gdz.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pey.yuanzhike.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vos.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vvx.snrcjt.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sjh.shuidangran.top

Go:   slices.Sort(arr)
来源：http://zma.xylfe.cn

Ruby: arr.sort
来源：http://uqg.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gtz.tanke756.top

[N03] 快速排序（分治示例）
来源：http://kbg.ywan-chungtsiang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mac.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://zmh.hnxiangtu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aut.kuanghao11.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eeu.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://neq.hnqzz.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ful.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yuy.shangyingyoupin.top

C#:   // 手写递归，或 Array.Sort
来源：http://nck.zhoulong.xyz

[N04] 斐波那契数列
来源：http://gxe.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ppp.zhoulong.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://itm.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gta.jqgufenzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mpa.tianlin.xyz


<!-- 参考信息 -->