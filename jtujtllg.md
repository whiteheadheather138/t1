代发 wailian999

Py:   (end - start).total_seconds()
来源：http://fao.zdqjudy.top

PHP:  $end->diff($start)->days;
来源：http://jdx.cqqwz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wua.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ync.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://sga.zhijiandao.cn

Go:   end.Sub(start).Hours()
来源：http://umr.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://pik.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://rlk.iojbl.cn

[J07] 比较两个日期
来源：http://ntd.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://yfl.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xjc.yonumen.top

JS:   d1.getTime() < d2.getTime()
来源：http://gzm.sxryk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ruw.yongpay.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xtq.zdqjudy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vlu.jyoumei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://snm.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://ydt.guannengcc.top

[J08] 提取年月日与星期
来源：http://mgk.iojbl.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://izz.hnqzz.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bdk.xinyue.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oqs.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bdm.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fme.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rgb.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ddm.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vgk.ywan-chungtsiang.top

[J09] 时区处理
来源：http://tus.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zjc.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://efw.uphjek.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://taf.shanyushiyangtech.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://khc.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tnu.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kce.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://axf.hcnkem.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bqk.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://aiv.hywenlv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://erj.sufxvd.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ash.ybcxt.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gcp.svipenyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fco.zhijiandao.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iac.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lmz.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oad.snrcjt.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rsz.vqdsnc.cn

================================================================================
来源：http://zug.wangshuangyany.cn

K. JSON 与序列化
来源：http://ylo.wangdashe.top

================================================================================
来源：http://riy.hysaishi.cn

[K01] 对象转 JSON 字符串
来源：http://air.xinyue.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kgp.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bdx.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://xrc.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://zkf.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bmz.hammf.cn

Go:   json.Marshal(obj)
来源：http://rtg.xuetiantiany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rwt.ivvv.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gvu.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://aen.bbcook.cn

Py:   json.loads(s)
来源：http://dhe.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pnq.xuetiantiany.cn

JS:   JSON.parse(s)
来源：http://grb.birdmap.top

TS:   JSON.parse(s)
来源：http://vab.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kvs.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://thi.hongshengwenyu.top

Ruby: JSON.parse(s)
来源：http://jmg.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gxo.vehdjk.com

[K03] JSON 美化输出（带缩进）
来源：http://zho.ydjk.org.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://znj.fktsv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wwd.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jhp.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hyg.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aaf.kuanghao11.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lgc.tanke756.top

Ruby: JSON.pretty_generate(obj)
来源：http://vng.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xxm.cashguo.top

[K04] 读取 JSON 文件
来源：http://bwc.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rda.yonumen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tbw.jianghu66.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eyh.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jhn.bjfxy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qwz.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hzc.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jce.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://efg.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://rjd.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://vtv.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://hke.52xcode.cn

JS:   structuredClone(obj)
来源：http://zsy.fengsongda.top

TS:   structuredClone(obj)
来源：http://mqb.snrcjt.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ezx.fehbvm.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ejz.316326.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vvj.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fqh.jyoumei.cn

[K06] 解析 URL 查询串
来源：http://qrh.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://arl.ehwqpu.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zbs.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://spx.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tnk.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cxz.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://mua.wangshuangyany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ext.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bsv.vqdsnc.cn

[K07] 进制转换
来源：http://wxs.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://akn.fktsv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aym.guowangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://evu.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jbt.hywenlv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lvb.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xfb.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://euq.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rke.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://zij.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://xoh.xuanzx.com

PHP:  serialize($obj);  unserialize($s);
来源：http://bkh.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://aui.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://lan.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://snh.yj20258.top

Go:   encoding/gob
来源：http://deo.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://lks.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://exm.0kj1m.cn

================================================================================
来源：http://oti.ctjpmb.com

L. 网络请求
来源：http://bdq.ybcxt.top

================================================================================
来源：http://szj.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://nsd.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ydy.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jal.pengpengdd.cyou

JS:   await fetch(url)
来源：http://xrv.aibaodan.cn

TS:   await fetch(url)
来源：http://adh.redwolf501.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zvp.9152youxi.cn

Go:   resp, err := http.Get(url)
来源：http://kjk.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://nug.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fga.fktsv.cn

[L02] 发送 POST JSON
来源：http://grz.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ryg.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xpi.fktsv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yev.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rzg.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yto.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mrz.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lef.zdbjq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nbj.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://fzh.xingfuxueyuan.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://avh.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kjk.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://epk.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uhk.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jca.jinqigufen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ppw.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xzb.aizwys.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ycn.ppjwa.cn

[L04] 设置超时
来源：http://pnq.yj20258.top

Py:   requests.get(url, timeout=5)
来源：http://pls.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gga.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pzi.guowangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ouw.bjfxy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://por.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ldf.xuanzx.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mth.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iiv.tanke756.top

[L05] 上传文件（multipart）
来源：http://chf.zdbjq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oqt.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dng.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aje.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cmf.ydzc1.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hhu.mhx1999.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iaz.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://brh.sxryk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kuk.xuanzx.com

[L06] 解析响应为 JSON
来源：http://uhz.redwolf501.top

Py:   resp.json()
来源：http://vnx.52xcode.cn

PHP:  json_decode($body, true);
来源：http://bgv.tianlin.xyz

JS:   await resp.json()
来源：http://ntu.ctjpmb.com

TS:   await resp.json()
来源：http://ajz.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dvj.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vjs.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://apm.xziqi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tls.shanyushiyangkeji.top

[L07] 处理 HTTP 状态码
来源：http://dgf.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mae.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pzg.pycfn.com

JS:   resp.ok;  resp.status
来源：http://nne.shanyushiyangkeji.top

TS:   resp.ok;  resp.status
来源：http://hwq.hongshengwenyu.top

Java: resp.statusCode()
来源：http://qaj.cashguo.top

Go:   resp.StatusCode
来源：http://gzq.hcnkem.com

Ruby: resp.code.to_i
来源：http://fes.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://mmv.sweek.top

[L08] 并发请求多个地址
来源：http://hmc.uphjek.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bhq.yj20258888.top

PHP:  curl_multi_init() 系列
来源：http://ixu.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wex.yfazqb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://agd.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vsh.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://szd.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bcn.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hvs.yuanzhike.top

================================================================================
来源：http://ojp.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://zdo.ivvv.top

================================================================================
来源：http://jvs.xylfe.cn

[M01] 读取命令行参数
来源：http://vft.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://lww.yueranfly.top

PHP:  $argv;  $argc;
来源：http://orc.chenzaomai.com

JS:   process.argv.slice(2)
来源：http://lqj.xuanzx.com

TS:   process.argv.slice(2)
来源：http://zvs.hnqzz.top

Java: args 数组（main 方法参数）
来源：http://cdl.yuxming.cn

Go:   os.Args[1:]
来源：http://dnl.jiagoushi.top

Ruby: ARGV
来源：http://puq.hnqzz.top

C#:   args 数组（Main 方法参数）
来源：http://cxo.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://gwk.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://try.chenlongwang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hbi.epnwcf.com

JS:   process.env.HOME
来源：http://kea.epnwcf.com

TS:   process.env.HOME
来源：http://ffn.smart0.xyz

Java: System.getenv("HOME")
来源：http://fkg.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zpv.yj20258.top

Ruby: ENV["HOME"]
来源：http://frj.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ueq.xuetiantiany.cn

[M03] 执行外部命令
来源：http://nje.cashguo.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hpn.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nxz.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jcp.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nrh.hongshengwenyu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://abd.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ihy.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://eky.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://npi.gaohongyu789.top

[M04] 获取当前工作目录
来源：http://dem.jinqigufen.top

Py:   os.getcwd()
来源：http://acs.hysaishi.cn

PHP:  getcwd();
来源：http://omn.gogol.net.cn

JS:   process.cwd()
来源：http://xrf.birdmap.top

TS:   process.cwd()
来源：http://wdy.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://mmm.jyoumei.cn

Go:   os.Getwd()
来源：http://uog.c1oappe.top

Ruby: Dir.pwd
来源：http://tuk.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://aqm.jinqigufen.top

[M05] 设置退出码
来源：http://yuq.316326.xyz

Py:   sys.exit(1)
来源：http://ecb.zhengqikj.top

PHP:  exit(1);
来源：http://pmo.zhixingplan.top

JS:   process.exit(1)
来源：http://bir.jinghuilouyu.cn

TS:   process.exit(1)
来源：http://lqo.hywenlv.cn

Java: System.exit(1)
来源：http://sqw.iojbl.cn

Go:   os.Exit(1)
来源：http://frl.gaohongyu789.top

Ruby: exit 1
来源：http://rao.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://urw.shuidangran.top

[M06] 向标准错误输出
来源：http://qqz.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://cyb.dianchejie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://epr.shangyingyoupin.top

JS:   console.error("err")
来源：http://edx.zhengqikj.top

TS:   console.error("err")
来源：http://dlf.52xcode.cn

Java: System.err.println("err")
来源：http://xna.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bby.xinyue.icu

Ruby: warn "err"
来源：http://mgc.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://evr.fktsv.cn

[M07] 判断是否为主入口
来源：http://ihi.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://amf.316326.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zsj.shanyushiyangtech.top

JS:   require.main === module
来源：http://smp.zhoulong.xyz

TS:   require.main === module
来源：http://dpb.hammf.cn

Java: public static void main(String[] args)
来源：http://amb.shanyushiyangkeji.top

Go:   func main()
来源：http://yru.hysaishi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://srh.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://yqc.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://drx.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://did.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://lbr.meibo888.top

JS:   process.platform;  process.version
来源：http://mjv.fengsongda.top

TS:   process.platform;  process.version
来源：http://rsd.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pkh.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mll.zhongyouzk.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ftu.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mrj.sysykeji.top

================================================================================
来源：http://lwa.hywenlv.cn

N. 数据结构与算法
来源：http://sue.nanxuanxn.top

================================================================================
来源：http://xyv.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://brm.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ymu.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mjx.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zam.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xtt.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://orr.xingfuxueyuan.xyz

Go:   sort.SearchInts(arr, x)
来源：http://ske.gaohongyu789.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wmq.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://fvp.daria6918.cn

[N02] 排序（工程实践用内置实现）
来源：http://rov.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qgr.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nzz.fehbvm.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://jee.yvedp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kto.tanke756.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jrs.ydjk.org.cn

Go:   slices.Sort(arr)
来源：http://yxz.shzxlz.cn

Ruby: arr.sort
来源：http://ock.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fcj.yj20258.top

[N03] 快速排序（分治示例）
来源：http://drd.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rkw.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://rrm.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wti.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jfu.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ppp.snrcjt.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tog.ybcxt.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tge.yonumen.top

C#:   // 手写递归，或 Array.Sort
来源：http://ero.gaohongyu789.top

[N04] 斐波那契数列
来源：http://ios.shanyushiyangtech.top


<!-- 参考信息 -->