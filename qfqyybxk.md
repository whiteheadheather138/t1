代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jrq.wangdashe.top

Ruby: Time.now + 7 * 86400
来源：http://hgd.zhaomingkeji.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://zkl.bjfxy.top

[J06] 计算两时间之差
来源：http://glq.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://iay.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://wzd.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://buv.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jda.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://iqm.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://wii.cheryme.top

Ruby: end - start                 # 返回秒数
来源：http://oem.shanyushiyangkeji.top

C#:   (end - start).TotalSeconds
来源：http://clh.gotoacloud.top

[J07] 比较两个日期
来源：http://hhm.ivvv.top

Py:   d1 < d2;  d1 == d2
来源：http://kwx.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hyd.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://mct.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://nzp.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xpa.yj20258888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tyv.fzhhl.top

Ruby: d1 < d2;  d1 == d2
来源：http://kry.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://rez.ehwqpu.com

[J08] 提取年月日与星期
来源：http://gec.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://men.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cit.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hfm.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mgq.ctjpmb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lfc.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jaj.yongpay.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lhk.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ihc.shanyushiyangtech.top

[J09] 时区处理
来源：http://ocq.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://utv.uphjek.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://avl.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vnm.sxryk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mhl.gaohongyu789.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uwc.ctjpmb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xic.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bvu.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gbs.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://iem.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://wbn.ivvv.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rev.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://usv.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mei.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sfq.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mkd.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yab.quarkkingdee.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gls.birdmap.top

================================================================================
来源：http://wfs.pycfn.com

K. JSON 与序列化
来源：http://jqb.jianghu66.top

================================================================================
来源：http://ura.wangshuangyany.cn

[K01] 对象转 JSON 字符串
来源：http://oke.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dyh.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tkh.wangdashe.top

JS:   JSON.stringify(obj)
来源：http://rkx.zhijiandao.cn

TS:   JSON.stringify(obj)
来源：http://fxp.tian-w.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ozz.xylfe.cn

Go:   json.Marshal(obj)
来源：http://xcp.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://txf.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zag.hesvh.cn

[K02] JSON 字符串转对象
来源：http://xkb.wangshuangyany.cn

Py:   json.loads(s)
来源：http://glx.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sez.pycfn.com

JS:   JSON.parse(s)
来源：http://ubg.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://fyx.sweek.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ilp.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://nxu.yj20258.top

Ruby: JSON.parse(s)
来源：http://rra.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mya.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://kic.zhoulong.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jbv.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jzg.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fgv.jinyuanbaomall.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ycw.bbcook.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wcv.epnwcf.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ejh.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://kai.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nwa.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://zds.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oww.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sjr.fktsv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://chs.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vgt.hcnkem.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jvf.xylfe.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hxg.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tng.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pni.epnwcf.com

[K05] 深拷贝对象
来源：http://ilj.sweek.top

Py:   copy.deepcopy(obj)
来源：http://muq.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://yqp.andypj.xyz

JS:   structuredClone(obj)
来源：http://jvu.yj202588.top

TS:   structuredClone(obj)
来源：http://qrp.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hzt.zhijiandao.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jvf.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://frr.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pwf.hongshengwenyu.top

[K06] 解析 URL 查询串
来源：http://zmo.yanxiufei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xcj.0kj1m.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pqx.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://swc.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://khm.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zfi.jqgfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vvt.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yiz.shanyushiyangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://unf.yonumen.top

[K07] 进制转换
来源：http://jff.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ypt.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iyj.xinyue.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://amr.smart0.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mgn.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xxv.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lfq.snrcjt.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wld.gaohongyu789.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://meq.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://vng.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://tcz.jinqigufen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://brw.iojbl.cn

JS:   v8.serialize(obj)        // Node
来源：http://fag.yuanzhike.top

TS:   v8.serialize(obj)        // Node
来源：http://jxd.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uak.yuxming.cn

Go:   encoding/gob
来源：http://hgi.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://ncx.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hrf.cashguo.top

================================================================================
来源：http://wcy.ivvv.top

L. 网络请求
来源：http://oek.hammf.cn

================================================================================
来源：http://zfp.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://wgn.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tvh.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aiz.ppjwa.cn

JS:   await fetch(url)
来源：http://kum.yj20258.top

TS:   await fetch(url)
来源：http://dim.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mww.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://gzf.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://owz.xuetiantiany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ppc.sjlbkw.cn

[L02] 发送 POST JSON
来源：http://sli.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fgy.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jug.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yts.fehbvm.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bab.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zbu.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jyk.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wqk.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://edn.yj20258888.top

[L03] 设置自定义请求头
来源：http://whr.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://npe.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zlk.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://amd.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ijs.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bhr.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lbn.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ajz.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jgb.redwolf501.top

[L04] 设置超时
来源：http://axa.fzhhl.top

Py:   requests.get(url, timeout=5)
来源：http://xcn.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wkl.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fpa.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fof.gogol.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gzj.yanxiufei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zkp.guannengcc.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sri.hfpthk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nob.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://xwz.havefunace.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bgy.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ymm.52xcode.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://msf.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pfx.yongpay.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vxq.jianghu66.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qto.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qcr.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ufc.fktsv.cn

[L06] 解析响应为 JSON
来源：http://aij.yongpay.top

Py:   resp.json()
来源：http://lnm.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://soo.hesvh.cn

JS:   await resp.json()
来源：http://bwi.hnxiangtu.top

TS:   await resp.json()
来源：http://bzn.fengsongda.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jec.tianlin.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ckn.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://xwg.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ucc.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://znz.dianchejie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aar.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lnb.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://pmc.hammf.cn

TS:   resp.ok;  resp.status
来源：http://mer.9152youxi.cn

Java: resp.statusCode()
来源：http://vfv.hcnkem.com

Go:   resp.StatusCode
来源：http://ksh.feifeiyinyue.top

Ruby: resp.code.to_i
来源：http://dcl.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://byi.meibo888.top

[L08] 并发请求多个地址
来源：http://ulr.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://niy.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://pul.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ffd.zycfv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ojg.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bft.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://krg.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pym.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ndk.meibo888.top

================================================================================
来源：http://fqv.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://ynv.9152youxi.cn

================================================================================
来源：http://nbf.fehbvm.com

[M01] 读取命令行参数
来源：http://nxf.nanxuanxn.top

Py:   sys.argv[1:]
来源：http://kfl.kuanghao11.cn

PHP:  $argv;  $argc;
来源：http://ggg.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://xhz.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://out.zdbjq.cn

Java: args 数组（main 方法参数）
来源：http://uhj.zdqjudy.top

Go:   os.Args[1:]
来源：http://crx.yj20258.top

Ruby: ARGV
来源：http://oon.chenzaomai.com

C#:   args 数组（Main 方法参数）
来源：http://aij.vehdjk.com

[M02] 读取环境变量
来源：http://lok.vqdsnc.cn

Py:   os.environ.get("HOME")
来源：http://kce.shangyingyoupin.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://afs.shanyushiyangtech.top

JS:   process.env.HOME
来源：http://trn.hnqzz.top

TS:   process.env.HOME
来源：http://wcr.fzhhl.top

Java: System.getenv("HOME")
来源：http://tbo.xuetiantiany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tez.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://vda.hysaishi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tba.shzxlz.cn

[M03] 执行外部命令
来源：http://muy.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pty.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xvo.feifeiyinyue.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xwu.yj202588.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cak.chenlongwang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tdc.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tvc.fengsongda.top

Ruby: system("ls -l");  `ls -l`
来源：http://ezo.zhiwuduotai.top

C#:   Process.Start("ls", "-l");
来源：http://bwx.xingfuxueyuan.xyz

[M04] 获取当前工作目录
来源：http://xlc.chenlongwang.top

Py:   os.getcwd()
来源：http://ars.fktsv.cn

PHP:  getcwd();
来源：http://yal.yvedp.cn

JS:   process.cwd()
来源：http://xks.ivvv.top

TS:   process.cwd()
来源：http://hrt.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://jmu.svipenyu.cn

Go:   os.Getwd()
来源：http://xfo.jlsjyb.cn

Ruby: Dir.pwd
来源：http://nod.xziqi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://enu.yueranfly.top

[M05] 设置退出码
来源：http://ifw.fktsv.cn

Py:   sys.exit(1)
来源：http://vmg.ppjwa.cn

PHP:  exit(1);
来源：http://ltx.gzhubu.top

JS:   process.exit(1)
来源：http://dsp.zhaomingkeji.xyz

TS:   process.exit(1)
来源：http://zli.tanke756.top

Java: System.exit(1)
来源：http://adi.sweek.top

Go:   os.Exit(1)
来源：http://qxg.jinqigfzy.top

Ruby: exit 1
来源：http://pxu.gzhubu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ovo.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://ydl.xuetiantiany.cn

Py:   print("err", file=sys.stderr)
来源：http://ywr.ppjwa.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nxi.yonumen.top

JS:   console.error("err")
来源：http://pzr.jianghu66.top

TS:   console.error("err")
来源：http://tva.havefunace.top

Java: System.err.println("err")
来源：http://ohd.zhoulong.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cux.andypj.xyz

Ruby: warn "err"
来源：http://twm.fehbvm.com

C#:   Console.Error.WriteLine("err")
来源：http://gfb.hywenlv.cn

[M07] 判断是否为主入口
来源：http://lwc.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://fvb.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qzt.hammf.cn

JS:   require.main === module
来源：http://wjd.jqgfzy.top

TS:   require.main === module
来源：http://iiv.guowangkeji.top

Java: public static void main(String[] args)
来源：http://hqq.iojbl.cn

Go:   func main()
来源：http://lqe.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oem.jqgufenzy.top

C#:   static void Main(string[] args)
来源：http://jdh.yonumen.top

[M08] 获取系统与运行时信息
来源：http://hqo.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://dkt.zycfv.cn

PHP:  PHP_OS;  phpversion();
来源：http://wni.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://tox.yj20258888.top

TS:   process.platform;  process.version
来源：http://zzb.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://umm.uphjek.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://jwh.yangfankeji.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://auk.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jjh.shanyushiyangtech.top

================================================================================
来源：http://kot.tian-w.cn

N. 数据结构与算法
来源：http://dyk.hnqzz.top

================================================================================
来源：http://ksp.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://xvw.shanyushiyangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://rfk.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bfs.tian-w.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nmx.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://orn.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://dzw.yonumen.top

Go:   sort.SearchInts(arr, x)
来源：http://wzx.chenlongwang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kty.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sol.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://qbn.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://wmi.bjfxy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zjd.ydzc1.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kqz.yongpay.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rrh.chenlongwang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gaj.wangdashe.top

Go:   slices.Sort(arr)
来源：http://wfu.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://ayp.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vqy.fktsv.cn

[N03] 快速排序（分治示例）
来源：http://bpn.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tnk.aizwys.cn

PHP:  // 递归实现，或用 usort
来源：http://amk.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yip.yuanzhike.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kwe.dianchejie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://owx.zycfv.cn


<!-- 参考信息 -->