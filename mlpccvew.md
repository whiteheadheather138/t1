代发 wailian999

Py:   (end - start).total_seconds()
来源：http://tvc.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://mkf.hcnkem.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://omy.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tet.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oli.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://jqo.ywan-chungtsiang.top

Ruby: end - start                 # 返回秒数
来源：http://bho.yanxiufei.cn

C#:   (end - start).TotalSeconds
来源：http://kkx.gogol.net.cn

[J07] 比较两个日期
来源：http://qor.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://erh.fanxiaobao.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zek.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fxj.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://ted.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vdo.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nzu.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jjv.aizwys.cn

C#:   d1 < d2;  d1 == d2
来源：http://cii.jyoumei.cn

[J08] 提取年月日与星期
来源：http://dcq.zycfv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zwh.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hzf.redwolf501.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ifb.cheryme.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xvz.dashuyun.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qmm.ydzc1.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zof.ppjwa.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rdy.yj20258.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bmf.fzhhl.top

[J09] 时区处理
来源：http://ahd.andypj.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yad.chenzaomai.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rpe.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://poq.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ftc.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cbc.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xbw.sxryk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dao.snrcjt.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mol.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://nps.svipenyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bpb.xylfe.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uwj.hcnkem.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ypb.52xcode.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lqc.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uip.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pxs.shuidangran.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sta.jiagoushi.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lre.hnqzz.top

================================================================================
来源：http://yti.yuanzhike.top

K. JSON 与序列化
来源：http://the.bbcook.cn

================================================================================
来源：http://tkn.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://oae.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ryk.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://olr.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://vil.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://zlt.yueranfly.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wod.yj20258888.top

Go:   json.Marshal(obj)
来源：http://dvm.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rmo.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bey.xuanzx.com

[K02] JSON 字符串转对象
来源：http://eyy.iojbl.cn

Py:   json.loads(s)
来源：http://lav.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zfh.shzxlz.cn

JS:   JSON.parse(s)
来源：http://xdq.zdqjudy.top

TS:   JSON.parse(s)
来源：http://acs.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jzy.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://fis.zycfv.cn

Ruby: JSON.parse(s)
来源：http://rvo.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wrg.hammf.cn

[K03] JSON 美化输出（带缩进）
来源：http://nhj.guannengcc.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mbf.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lya.redwolf501.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mtz.c1oappe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hgm.meibo888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ues.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cae.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://mlw.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qvz.daxiang520.top

[K04] 读取 JSON 文件
来源：http://ett.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zad.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nsp.wangdashe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://myu.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mtr.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vbh.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oog.cheryme.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ovn.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tkp.guannengcc.top

[K05] 深拷贝对象
来源：http://kad.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://hqx.gotoacloud.top

PHP:  unserialize(serialize($obj));
来源：http://ykt.nanxuanxn.top

JS:   structuredClone(obj)
来源：http://ekl.guowangkeji.top

TS:   structuredClone(obj)
来源：http://mzu.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wlc.yuxming.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pca.cucudq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kpd.52xcode.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fuq.hnqzz.top

[K06] 解析 URL 查询串
来源：http://nnt.ydzc1.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vcr.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bot.bbcook.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jiy.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dhl.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bod.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://uhy.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://prs.kuanghao11.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xwd.kuanghao11.cn

[K07] 进制转换
来源：http://hhy.cheryme.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mpa.zhiwuduotai.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lhh.cheryme.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eak.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://umu.cucudq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://siu.redwolf501.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ocy.jinqigfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pyh.yonumen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oci.bjfxy.top

[K08] 二进制序列化（非 JSON）
来源：http://jks.hnqzz.top

Py:   pickle.dumps(obj)
来源：http://jzz.jianghu66.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vge.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://clt.jinqigfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://brg.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vah.havefunace.top

Go:   encoding/gob
来源：http://vjx.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://nfv.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aee.hfpthk.cn

================================================================================
来源：http://srg.shuidangran.top

L. 网络请求
来源：http://bmk.tarul.cn

================================================================================
来源：http://vkf.cashguo.top

[L01] 发送 GET 请求
来源：http://qmb.sxryk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vjv.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zit.birdmap.top

JS:   await fetch(url)
来源：http://ihx.ivvv.top

TS:   await fetch(url)
来源：http://aym.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ikt.chenlongwang.top

Go:   resp, err := http.Get(url)
来源：http://cpz.aibaodan.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qlm.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hse.xinyue.icu

[L02] 发送 POST JSON
来源：http://ltc.316326.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://xfb.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xmw.snrcjt.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fqq.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ppt.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://use.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://trj.shangyingyoupin.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rxz.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mbv.hysaishi.cn

[L03] 设置自定义请求头
来源：http://dpl.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://exy.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://avm.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ian.daria6918.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qer.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qca.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yff.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rzq.ppjwa.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fuu.jinqigfzy.top

[L04] 设置超时
来源：http://chb.xinyue.icu

Py:   requests.get(url, timeout=5)
来源：http://wph.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hda.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rxt.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wkw.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dkj.bjfxy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xiz.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://owq.gzhubu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zst.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://dmc.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pyk.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fmz.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fvk.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qqw.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://joa.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://buu.ywan-chungtsiang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eal.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kmw.jinyuanbaomall.cn

[L06] 解析响应为 JSON
来源：http://vio.guannengcc.top

Py:   resp.json()
来源：http://biq.dianchejie.cn

PHP:  json_decode($body, true);
来源：http://mhf.yanxiufei.cn

JS:   await resp.json()
来源：http://qzl.yueranfly.top

TS:   await resp.json()
来源：http://xvh.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cko.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xcc.shanyushiyangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://ski.bbcook.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hog.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://mvo.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cpm.ivvv.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mrm.cheryme.top

JS:   resp.ok;  resp.status
来源：http://ppq.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://jvb.ppjwa.cn

Java: resp.statusCode()
来源：http://tmf.sufxvd.cn

Go:   resp.StatusCode
来源：http://rvv.chenzaomai.com

Ruby: resp.code.to_i
来源：http://iaz.guowangkeji.top

C#:   (int)resp.StatusCode
来源：http://iud.fktsv.cn

[L08] 并发请求多个地址
来源：http://zdk.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yyz.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://kxc.yueranfly.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mzr.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lhb.ivvv.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lct.xuetiantiany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nfm.sufxvd.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://unb.cashguo.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jzn.zdbjq.cn

================================================================================
来源：http://lve.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://byn.zhixingplan.top

================================================================================
来源：http://cjd.sxryk.cn

[M01] 读取命令行参数
来源：http://ufe.redwolf501.top

Py:   sys.argv[1:]
来源：http://vui.sxryk.cn

PHP:  $argv;  $argc;
来源：http://ria.yvedp.cn

JS:   process.argv.slice(2)
来源：http://obe.pycfn.com

TS:   process.argv.slice(2)
来源：http://olp.ydjk.org.cn

Java: args 数组（main 方法参数）
来源：http://ctl.daria6918.cn

Go:   os.Args[1:]
来源：http://ckf.pycfn.com

Ruby: ARGV
来源：http://sjd.vqdsnc.cn

C#:   args 数组（Main 方法参数）
来源：http://chr.jinyuanbaomall.cn

[M02] 读取环境变量
来源：http://sif.hfpthk.cn

Py:   os.environ.get("HOME")
来源：http://pxx.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://flu.guannengcc.top

JS:   process.env.HOME
来源：http://tul.shuidangran.top

TS:   process.env.HOME
来源：http://vjg.hcnkem.com

Java: System.getenv("HOME")
来源：http://clx.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bac.redwolf501.top

Ruby: ENV["HOME"]
来源：http://tbl.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jig.xuetiantiany.cn

[M03] 执行外部命令
来源：http://dtq.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kcd.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eve.hcnkem.com

JS:   child_process.execSync("ls -l").toString()
来源：http://qae.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://kvy.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fwt.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://avq.zhixingplan.top

Ruby: system("ls -l");  `ls -l`
来源：http://qun.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://bui.havefunace.top

[M04] 获取当前工作目录
来源：http://uza.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://hrl.yueranfly.top

PHP:  getcwd();
来源：http://pua.yueranfly.top

JS:   process.cwd()
来源：http://atu.cheryme.top

TS:   process.cwd()
来源：http://jil.zhijiandao.cn

Java: Path.of("").toAbsolutePath()
来源：http://ibz.xylfe.cn

Go:   os.Getwd()
来源：http://crc.xinyue.icu

Ruby: Dir.pwd
来源：http://gza.ctjpmb.com

C#:   Directory.GetCurrentDirectory()
来源：http://vxd.316326.xyz

[M05] 设置退出码
来源：http://jij.hywenlv.cn

Py:   sys.exit(1)
来源：http://rfe.nwbrower.top

PHP:  exit(1);
来源：http://cny.quarkkingdee.top

JS:   process.exit(1)
来源：http://djg.tanke756.top

TS:   process.exit(1)
来源：http://amt.shzxlz.cn

Java: System.exit(1)
来源：http://uev.fktsv.cn

Go:   os.Exit(1)
来源：http://tsj.yongpay.top

Ruby: exit 1
来源：http://qqc.daria6918.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zpx.zdbjq.cn

[M06] 向标准错误输出
来源：http://win.cdnleiting.top

Py:   print("err", file=sys.stderr)
来源：http://shu.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cgg.ehwqpu.com

JS:   console.error("err")
来源：http://pmu.wangdashe.top

TS:   console.error("err")
来源：http://ntt.jinqigufen.top

Java: System.err.println("err")
来源：http://qan.nanxuanxn.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oix.mhx1999.top

Ruby: warn "err"
来源：http://cck.jianghu66.top

C#:   Console.Error.WriteLine("err")
来源：http://huc.dashuyun.cn

[M07] 判断是否为主入口
来源：http://tmm.cheryme.top

Py:   if __name__ == "__main__":
来源：http://fzk.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qbb.nanxinkj.top

JS:   require.main === module
来源：http://ype.hongshengwenyu.top

TS:   require.main === module
来源：http://euu.ppjwa.cn

Java: public static void main(String[] args)
来源：http://bea.jianghu66.top

Go:   func main()
来源：http://den.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lke.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://wth.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://tjj.vehdjk.com

Py:   platform.system();  platform.python_version()
来源：http://fiq.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://fng.sweek.top

JS:   process.platform;  process.version
来源：http://taq.chenjidiqi.icu

TS:   process.platform;  process.version
来源：http://upe.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gzc.9152youxi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cmh.jlsjyb.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mwe.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eqs.gaohongyu789.top

================================================================================
来源：http://cvp.yj20258.top

N. 数据结构与算法
来源：http://huu.hcnkem.com

================================================================================
来源：http://uqj.birdmap.top

[N01] 二分查找（有序数组）
来源：http://oei.ydzc1.top

Py:   bisect.bisect_left(arr, x)
来源：http://ola.vqdsnc.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zej.tanke756.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ygv.ybcxt.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xrk.bjfxy.top

Java: Arrays.binarySearch(arr, x)
来源：http://inx.guannengcc.top

Go:   sort.SearchInts(arr, x)
来源：http://ykj.epnwcf.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://jkp.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://koq.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://psp.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://pcr.yuanzhike.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jek.daxiang520.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jxo.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://mgv.316326.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://djj.daria6918.cn

Go:   slices.Sort(arr)
来源：http://tpk.zhengqikj.top

Ruby: arr.sort
来源：http://nmc.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://bth.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://zki.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pqc.gaohongyu789.top

PHP:  // 递归实现，或用 usort
来源：http://inb.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ghl.52xcode.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://otc.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ihu.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gld.yfazqb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lum.cdnleiting.top

C#:   // 手写递归，或 Array.Sort
来源：http://qhe.ybcxt.top

[N04] 斐波那契数列
来源：http://tpt.tanke756.top


<!-- 参考信息 -->