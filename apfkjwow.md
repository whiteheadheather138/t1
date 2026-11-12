代发 wailian999

[J07] 比较两个日期
来源：http://xdn.ivvv.top

Py:   d1 < d2;  d1 == d2
来源：http://lgj.ydjk.org.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ysy.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://jct.xuanzx.com

TS:   d1.getTime() < d2.getTime()
来源：http://pte.shuidangran.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mhg.yuxming.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nqz.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dyg.jinqigfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://vyz.shuidangran.top

[J08] 提取年月日与星期
来源：http://rnj.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://aja.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jsl.shangyingyoupin.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kdf.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://psf.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pvj.hywenlv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lff.cdnleiting.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xqz.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kkq.shzxlz.cn

[J09] 时区处理
来源：http://auz.bjfxy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://awn.tian-w.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uwy.zhengqikj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fyq.yueranfly.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pbu.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wzm.mhx1999.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gno.svipenyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gmn.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nyn.hesvh.cn

[J10] 取今天 / 本月第一天
来源：http://khy.yonumen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://syl.yonumen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pbf.uphjek.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wrf.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vta.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sgb.yongpay.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ypx.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tth.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ptp.ppjwa.cn

================================================================================
来源：http://lhg.ydjk.org.cn

K. JSON 与序列化
来源：http://vau.yongpay.top

================================================================================
来源：http://ngw.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://wyi.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mje.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xyn.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://ohp.xinyue.icu

TS:   JSON.stringify(obj)
来源：http://beg.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lwv.tanke756.top

Go:   json.Marshal(obj)
来源：http://zgm.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://azx.chenlongwang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kbl.zhiwuduotai.top

[K02] JSON 字符串转对象
来源：http://opj.sweek.top

Py:   json.loads(s)
来源：http://omh.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lry.zhijiandao.cn

JS:   JSON.parse(s)
来源：http://gtf.shanyushiyangtech.top

TS:   JSON.parse(s)
来源：http://hbh.316326.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qgl.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://ehz.tanke756.top

Ruby: JSON.parse(s)
来源：http://kph.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xdv.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://qrz.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tmk.c1oappe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qba.jqgufenzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jcu.pycfn.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ukp.hfpthk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rth.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kqv.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wdh.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wyr.daxiang520.top

[K04] 读取 JSON 文件
来源：http://edk.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://icl.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zup.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://otb.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://deq.gaohongyu789.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zhp.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yuu.zhijiandao.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yib.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vtr.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://fbo.nanxinkj.top

Py:   copy.deepcopy(obj)
来源：http://nsq.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://aur.hysaishi.cn

JS:   structuredClone(obj)
来源：http://cke.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://smj.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pyv.yvedp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rha.gogol.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ybc.bbcook.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xfz.fengsongda.top

[K06] 解析 URL 查询串
来源：http://ahl.kuanghao11.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qlo.ywan-chungtsiang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pju.yj20258888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rit.pycfn.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qzr.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uzt.yuxming.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vgm.hysaishi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bwo.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ghc.ctjpmb.com

[K07] 进制转换
来源：http://rzp.ywan-chungtsiang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wbw.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yye.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mgv.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nya.dianchejie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lvo.ywan-chungtsiang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ufk.iojbl.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ytm.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oim.nwbrower.top

[K08] 二进制序列化（非 JSON）
来源：http://nhp.chenjidiqi.icu

Py:   pickle.dumps(obj)
来源：http://nnn.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uuv.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://tih.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://ypz.vqdsnc.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hun.sysykeji.top

Go:   encoding/gob
来源：http://pug.c1oappe.top

Ruby: Marshal.dump(obj)
来源：http://kfl.ybcxt.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jmx.yangfankeji.com

================================================================================
来源：http://zyr.guannengcc.top

L. 网络请求
来源：http://shf.fehbvm.com

================================================================================
来源：http://xaw.xylfe.cn

[L01] 发送 GET 请求
来源：http://omw.bbcook.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vsu.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vcs.xinyue.icu

JS:   await fetch(url)
来源：http://lso.hongshengwenyu.top

TS:   await fetch(url)
来源：http://bwe.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fef.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://pcd.aizwys.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://akb.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wwa.daxiang520.top

[L02] 发送 POST JSON
来源：http://xob.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://cci.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hrg.zhengqikj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vne.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ale.cashguo.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lnr.kuanghao11.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yua.sjlbkw.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kbc.redwolf501.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zyn.gotoacloud.top

[L03] 设置自定义请求头
来源：http://mts.bbcook.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iwk.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ovo.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://czg.0kj1m.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ghm.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wgq.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aui.shzxlz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bdx.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lhy.vqdsnc.cn

[L04] 设置超时
来源：http://ocy.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://uqh.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uuu.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ykr.birdmap.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qiv.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yka.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gix.jianghu66.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dsq.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://flh.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://eug.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zpr.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cax.shuidangran.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xtk.tianlin.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eiz.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qns.hnxiangtu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tjl.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mlx.shanyushiyangtech.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vvt.52xcode.cn

[L06] 解析响应为 JSON
来源：http://twe.zycfv.cn

Py:   resp.json()
来源：http://ncb.xuanzx.com

PHP:  json_decode($body, true);
来源：http://twy.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://her.pycfn.com

TS:   await resp.json()
来源：http://snf.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://szf.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wvk.vehdjk.com

Ruby: JSON.parse(resp.body)
来源：http://bka.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rqq.zdqjudy.top

[L07] 处理 HTTP 状态码
来源：http://tlv.zhongyouzk.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ndq.snrcjt.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tbt.fehbvm.com

JS:   resp.ok;  resp.status
来源：http://lrx.pengpengdd.cyou

TS:   resp.ok;  resp.status
来源：http://ouc.cucudq.cn

Java: resp.statusCode()
来源：http://ano.cqqwz.cn

Go:   resp.StatusCode
来源：http://evv.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://bkt.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://eug.gaohongyu789.top

[L08] 并发请求多个地址
来源：http://imb.jqgfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ccu.zhongyouzk.top

PHP:  curl_multi_init() 系列
来源：http://iif.nanxinkj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dyo.52xcode.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wre.ybcxt.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://daq.dashuyun.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fwi.yonumen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xdk.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ala.epnwcf.com

================================================================================
来源：http://tnt.jinqigufen.top

M. 命令行 / 进程 / 环境
来源：http://fom.hysaishi.cn

================================================================================
来源：http://qwh.gaohongyu789.top

[M01] 读取命令行参数
来源：http://jwf.yonumen.top

Py:   sys.argv[1:]
来源：http://ppw.sxryk.cn

PHP:  $argv;  $argc;
来源：http://pnh.zdqjudy.top

JS:   process.argv.slice(2)
来源：http://und.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://nty.chenlongwang.top

Java: args 数组（main 方法参数）
来源：http://oqv.jianghu66.top

Go:   os.Args[1:]
来源：http://qst.sweek.top

Ruby: ARGV
来源：http://hzj.yvedp.cn

C#:   args 数组（Main 方法参数）
来源：http://gze.kuanghao11.cn

[M02] 读取环境变量
来源：http://ptb.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://raj.zhongyouzk.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://erc.zhoulong.xyz

JS:   process.env.HOME
来源：http://mww.cucudq.cn

TS:   process.env.HOME
来源：http://pvl.fanxiaobao.xyz

Java: System.getenv("HOME")
来源：http://veb.zhixingplan.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xtd.yvedp.cn

Ruby: ENV["HOME"]
来源：http://qdd.hcnkem.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lhr.fehbvm.com

[M03] 执行外部命令
来源：http://tyt.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tzh.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://puj.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sxc.yanxiufei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xvu.9152youxi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cwg.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iux.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://mrl.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://syp.tarul.cn

[M04] 获取当前工作目录
来源：http://bmd.jinqigfzy.top

Py:   os.getcwd()
来源：http://kxf.jqgufenzy.top

PHP:  getcwd();
来源：http://egk.yanxiufei.cn

JS:   process.cwd()
来源：http://zxo.cheryme.top

TS:   process.cwd()
来源：http://mht.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://csa.dianchejie.cn

Go:   os.Getwd()
来源：http://gjp.sufxvd.cn

Ruby: Dir.pwd
来源：http://ubd.nanxuanxn.top

C#:   Directory.GetCurrentDirectory()
来源：http://chx.hysaishi.cn

[M05] 设置退出码
来源：http://bzv.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://xsh.snrcjt.cn

PHP:  exit(1);
来源：http://pck.yonumen.top

JS:   process.exit(1)
来源：http://fzs.haohaochexian.top

TS:   process.exit(1)
来源：http://wjn.chenzaomai.com

Java: System.exit(1)
来源：http://pgu.hysaishi.cn

Go:   os.Exit(1)
来源：http://pct.nanxuanxn.top

Ruby: exit 1
来源：http://rvp.nwbrower.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yys.xylfe.cn

[M06] 向标准错误输出
来源：http://oss.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://aly.bbcook.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ndr.dashuyun.cn

JS:   console.error("err")
来源：http://one.nanxinkj.top

TS:   console.error("err")
来源：http://efn.9152youxi.cn

Java: System.err.println("err")
来源：http://cvk.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cfo.zhaomingkeji.xyz

Ruby: warn "err"
来源：http://pcu.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://nch.gotoacloud.top

[M07] 判断是否为主入口
来源：http://iuy.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://kfc.xuetiantiany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lxx.hesvh.cn

JS:   require.main === module
来源：http://mhq.quarkkingdee.top

TS:   require.main === module
来源：http://wdk.tianlin.xyz

Java: public static void main(String[] args)
来源：http://jdr.xuanzx.com

Go:   func main()
来源：http://amn.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bni.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://zdv.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://trq.hnqzz.top

Py:   platform.system();  platform.python_version()
来源：http://vzo.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://nfl.wangdashe.top

JS:   process.platform;  process.version
来源：http://rya.bjfxy.top

TS:   process.platform;  process.version
来源：http://zfg.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://irr.jinqigfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lrb.hfpthk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tvt.dianchejie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jgv.yj20258.top

================================================================================
来源：http://hjf.hysaishi.cn

N. 数据结构与算法
来源：http://fla.chenjidiqi.icu

================================================================================
来源：http://fam.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://vxk.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://qzz.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qko.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://udx.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gbj.316326.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://tro.ppjwa.cn

Go:   sort.SearchInts(arr, x)
来源：http://uow.ehwqpu.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://acq.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://dnb.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://zsd.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://kpp.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hdf.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://dmd.vqdsnc.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ocd.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cxq.zhaomingkeji.xyz

Go:   slices.Sort(arr)
来源：http://xaw.dianchejie.cn

Ruby: arr.sort
来源：http://hfl.chenzaomai.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ftz.tarul.cn

[N03] 快速排序（分治示例）
来源：http://qra.c1oappe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tmp.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://omm.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lsj.chenjidiqi.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ane.yonumen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ldz.vehdjk.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nqv.jlsjyb.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ehb.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://qbj.zhongyouzk.top

[N04] 斐波那契数列
来源：http://dvp.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mnw.xinyue.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ywx.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aos.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jyi.xingfuxueyuan.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ztr.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wpe.guowangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bgh.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wei.daxiang520.top


<!-- 参考信息 -->