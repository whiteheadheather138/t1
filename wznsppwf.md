代发 wailian999

Py:   (end - start).total_seconds()
来源：http://xyf.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://dqn.sjlbkw.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iht.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zot.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://oac.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://hfa.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://ijs.hongshengwenyu.top

C#:   (end - start).TotalSeconds
来源：http://ihv.xuetiantiany.cn

[J07] 比较两个日期
来源：http://uwn.meibo888.top

Py:   d1 < d2;  d1 == d2
来源：http://bqx.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iqb.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ntv.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://bvl.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://utl.zhiwuduotai.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://svg.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kai.shzxlz.cn

C#:   d1 < d2;  d1 == d2
来源：http://ilq.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://spb.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ssa.jinqigufen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tzc.kuanghao11.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rur.cheryme.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aec.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hjb.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nys.birdmap.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lkr.gzhubu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qkg.xuanzx.com

[J09] 时区处理
来源：http://bdq.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nwh.vehdjk.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mna.ppjwa.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aou.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wbu.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qtv.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qol.hnqzz.top

Ruby: Time.now.getlocal("+08:00")
来源：http://juf.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rgr.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://fac.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qft.feifeiyinyue.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dvs.yonumen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kcm.jinyuanbaomall.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dna.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bjy.zhongyouzk.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wyj.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eys.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ceb.tian-w.cn

================================================================================
来源：http://xge.hfpthk.cn

K. JSON 与序列化
来源：http://wrh.gaohongyu789.top

================================================================================
来源：http://isg.daria6918.cn

[K01] 对象转 JSON 字符串
来源：http://pce.xuanzx.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vmf.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cwx.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://uzy.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://dlj.jianghu66.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xxw.jianghu66.top

Go:   json.Marshal(obj)
来源：http://kin.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://plf.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ewt.chenjidiqi.icu

[K02] JSON 字符串转对象
来源：http://hxl.zhongyouzk.top

Py:   json.loads(s)
来源：http://tad.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://omk.daria6918.cn

JS:   JSON.parse(s)
来源：http://gwp.daria6918.cn

TS:   JSON.parse(s)
来源：http://hwr.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qlx.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://ezq.hysaishi.cn

Ruby: JSON.parse(s)
来源：http://ebt.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jmh.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://kyy.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zni.zhijiandao.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nlc.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hhj.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://exa.yongpay.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://edw.52xcode.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://isv.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://itp.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kyh.zdqjudy.top

[K04] 读取 JSON 文件
来源：http://raz.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pjh.ywan-chungtsiang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pld.sxryk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uts.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hjj.jinqigfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ktu.tanke756.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dxl.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rlw.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wvx.jianghu66.top

[K05] 深拷贝对象
来源：http://klz.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://izo.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://bmo.wangshuangyany.cn

JS:   structuredClone(obj)
来源：http://ony.yj20258888.top

TS:   structuredClone(obj)
来源：http://tzz.haohaochexian.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ikj.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cqc.yongpay.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gdd.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oev.feifeiyinyue.top

[K06] 解析 URL 查询串
来源：http://mnw.shanyushiyangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wnp.cucudq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bfp.hfpthk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jpj.shuidangran.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ttl.zhixingplan.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rrp.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mlx.yuxming.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tnt.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tiv.cashguo.top

[K07] 进制转换
来源：http://mcb.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://izq.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://exn.guowangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ljy.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ydv.c1oappe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pvf.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bgm.hcnkem.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cyy.sysykeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eyl.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://vfu.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://eav.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xto.nanxuanxn.top

JS:   v8.serialize(obj)        // Node
来源：http://ehr.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://znq.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uqd.xuetiantiany.cn

Go:   encoding/gob
来源：http://noc.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://qro.tianlin.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ahd.zhiwuduotai.top

================================================================================
来源：http://afp.birdmap.top

L. 网络请求
来源：http://jbo.haohaochexian.top

================================================================================
来源：http://gib.yj20258888.top

[L01] 发送 GET 请求
来源：http://sla.ctjpmb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zkv.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://msx.xuanzx.com

JS:   await fetch(url)
来源：http://ctr.aizwys.cn

TS:   await fetch(url)
来源：http://ghk.redwolf501.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://opc.cheryme.top

Go:   resp, err := http.Get(url)
来源：http://xcv.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hdo.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ulv.9152youxi.cn

[L02] 发送 POST JSON
来源：http://nex.gzhubu.top

Py:   requests.post(url, json={"a": 1})
来源：http://njq.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lkg.shzxlz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bcu.jqgufenzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sbe.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cjm.yangfankeji.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hlr.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eem.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wjy.iojbl.cn

[L03] 设置自定义请求头
来源：http://duc.fzhhl.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fxi.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ydu.xuetiantiany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://muo.hcnkem.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ety.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dhe.316326.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fwt.xuanzx.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://alj.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lfm.jyoumei.cn

[L04] 设置超时
来源：http://rgm.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://qde.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ykw.jinqigufen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cav.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fby.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lim.jinghuilouyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xkl.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lcm.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qod.birdmap.top

[L05] 上传文件（multipart）
来源：http://psq.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rew.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vqj.xinyue.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yqm.hcnkem.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uvp.yuanzhike.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bdl.shanyushiyangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://grq.sysykeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://udp.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qux.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://aex.iojbl.cn

Py:   resp.json()
来源：http://sdp.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://mll.fanxiaobao.xyz

JS:   await resp.json()
来源：http://ieq.jinghuilouyu.cn

TS:   await resp.json()
来源：http://hbx.daxiang520.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ipw.andypj.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cot.316326.xyz

Ruby: JSON.parse(resp.body)
来源：http://cvm.pengpengdd.cyou

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qtd.hnxiangtu.top

[L07] 处理 HTTP 状态码
来源：http://npx.shanyushiyangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xwv.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dwt.hesvh.cn

JS:   resp.ok;  resp.status
来源：http://aos.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://bxm.jqgufenzy.top

Java: resp.statusCode()
来源：http://vqg.haohaochexian.top

Go:   resp.StatusCode
来源：http://tfi.316326.xyz

Ruby: resp.code.to_i
来源：http://yhj.yongpay.top

C#:   (int)resp.StatusCode
来源：http://tbd.chenlongwang.top

[L08] 并发请求多个地址
来源：http://quo.hammf.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zrt.xuanzx.com

PHP:  curl_multi_init() 系列
来源：http://tgr.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eqs.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kuo.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://znc.cqqwz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vbe.cqqwz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://drm.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lgr.hnqzz.top

================================================================================
来源：http://ciq.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://gmj.52xcode.cn

================================================================================
来源：http://lac.jianghu66.top

[M01] 读取命令行参数
来源：http://vhm.ppjwa.cn

Py:   sys.argv[1:]
来源：http://ctq.nwbrower.top

PHP:  $argv;  $argc;
来源：http://hxd.aibaodan.cn

JS:   process.argv.slice(2)
来源：http://ogb.cqqwz.cn

TS:   process.argv.slice(2)
来源：http://pgw.cucudq.cn

Java: args 数组（main 方法参数）
来源：http://enj.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://oql.hywenlv.cn

Ruby: ARGV
来源：http://dja.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://xnt.gogol.net.cn

[M02] 读取环境变量
来源：http://lwv.svipenyu.cn

Py:   os.environ.get("HOME")
来源：http://eri.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pei.xinyue.icu

JS:   process.env.HOME
来源：http://irr.ppjwa.cn

TS:   process.env.HOME
来源：http://iif.iojbl.cn

Java: System.getenv("HOME")
来源：http://uhj.sxryk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hrt.cheryme.top

Ruby: ENV["HOME"]
来源：http://tvx.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jwm.yuanzhike.top

[M03] 执行外部命令
来源：http://htv.guannengcc.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://clf.smart0.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kkm.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vkz.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://aif.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fjk.hesvh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bou.fzhhl.top

Ruby: system("ls -l");  `ls -l`
来源：http://hvy.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://dfm.jyoumei.cn

[M04] 获取当前工作目录
来源：http://bzx.sufxvd.cn

Py:   os.getcwd()
来源：http://bji.cqqwz.cn

PHP:  getcwd();
来源：http://blj.vqdsnc.cn

JS:   process.cwd()
来源：http://qqw.cdnleiting.top

TS:   process.cwd()
来源：http://luf.xinyue.icu

Java: Path.of("").toAbsolutePath()
来源：http://tmz.yfazqb.com

Go:   os.Getwd()
来源：http://mjh.ivvv.top

Ruby: Dir.pwd
来源：http://qrd.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://tnn.jiagoushi.top

[M05] 设置退出码
来源：http://eie.fktsv.cn

Py:   sys.exit(1)
来源：http://kji.hnqzz.top

PHP:  exit(1);
来源：http://fix.shanyushiyangtech.top

JS:   process.exit(1)
来源：http://vfp.guannengcc.top

TS:   process.exit(1)
来源：http://uge.tanke756.top

Java: System.exit(1)
来源：http://pce.epnwcf.com

Go:   os.Exit(1)
来源：http://nom.aibaodan.cn

Ruby: exit 1
来源：http://yfj.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wpi.gotoacloud.top

[M06] 向标准错误输出
来源：http://ncd.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://rmz.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fgn.daxiang520.top

JS:   console.error("err")
来源：http://amw.ywan-chungtsiang.top

TS:   console.error("err")
来源：http://jqs.cashguo.top

Java: System.err.println("err")
来源：http://erg.hfpthk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bhw.nwbrower.top

Ruby: warn "err"
来源：http://dwz.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://drg.hcnkem.com

[M07] 判断是否为主入口
来源：http://yuf.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://igd.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yqw.ppjwa.cn

JS:   require.main === module
来源：http://gwl.hywenlv.cn

TS:   require.main === module
来源：http://vlo.yongpay.top

Java: public static void main(String[] args)
来源：http://mou.jyoumei.cn

Go:   func main()
来源：http://boj.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dnv.meibo888.top

C#:   static void Main(string[] args)
来源：http://fkp.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://gng.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://ccl.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://sug.fzhhl.top

JS:   process.platform;  process.version
来源：http://dmg.jinghuilouyu.cn

TS:   process.platform;  process.version
来源：http://plb.ehwqpu.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jww.nanxinkj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://buq.zdqjudy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aup.guowangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kqx.ivvv.top

================================================================================
来源：http://kln.birdmap.top

N. 数据结构与算法
来源：http://dxt.hfpthk.cn

================================================================================
来源：http://zom.svipenyu.cn

[N01] 二分查找（有序数组）
来源：http://pxn.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cbf.zdqjudy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pci.c1oappe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://usa.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vqk.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://xbj.zhaomingkeji.xyz

Go:   sort.SearchInts(arr, x)
来源：http://uln.yj202588.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hrw.pycfn.com

C#:   Array.BinarySearch(arr, x)
来源：http://ajm.vehdjk.com

[N02] 排序（工程实践用内置实现）
来源：http://sbe.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://jho.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zhe.yanxiufei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nmf.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dea.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mpr.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://bqb.cheryme.top

Ruby: arr.sort
来源：http://tgx.wangdashe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dhw.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://jgv.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tpk.yj20258888.top

PHP:  // 递归实现，或用 usort
来源：http://tau.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zlh.ehwqpu.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kya.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iex.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://epg.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sqq.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://ryb.daria6918.cn

[N04] 斐波那契数列
来源：http://msv.yanxiufei.cn


<!-- 参考信息 -->