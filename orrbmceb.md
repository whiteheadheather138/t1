代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://ltr.nwbrower.top

Go:   end.Sub(start).Hours()
来源：http://uiz.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://jge.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://vie.yanxiufei.cn

[J07] 比较两个日期
来源：http://hnb.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://guh.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://agg.cdnleiting.top

JS:   d1.getTime() < d2.getTime()
来源：http://rcf.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://myq.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gea.mhx1999.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nrz.xziqi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qws.guannengcc.top

C#:   d1 < d2;  d1 == d2
来源：http://smh.sysykeji.top

[J08] 提取年月日与星期
来源：http://wew.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://llq.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xuq.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://enm.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rsv.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vmx.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jtn.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nyo.gogol.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://quj.shzxlz.cn

[J09] 时区处理
来源：http://gcq.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hhk.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://weu.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tjq.xylfe.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pqa.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ndv.jqgufenzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xdx.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://slw.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dch.zhiwuduotai.top

[J10] 取今天 / 本月第一天
来源：http://pvv.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hsp.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bsy.bbcook.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lfb.sufxvd.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://deh.yj20258888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wld.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fbt.fengsongda.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mzk.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kwq.chenzaomai.com

================================================================================
来源：http://xml.chenzaomai.com

K. JSON 与序列化
来源：http://hru.wangdashe.top

================================================================================
来源：http://hbi.jiagoushi.top

[K01] 对象转 JSON 字符串
来源：http://jdy.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://clg.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tql.jlsjyb.cn

JS:   JSON.stringify(obj)
来源：http://znn.aibaodan.cn

TS:   JSON.stringify(obj)
来源：http://dib.ppjwa.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nkl.smart0.xyz

Go:   json.Marshal(obj)
来源：http://cxk.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rpk.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gwm.gzhubu.top

[K02] JSON 字符串转对象
来源：http://wrk.guannengcc.top

Py:   json.loads(s)
来源：http://ghx.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xmv.52xcode.cn

JS:   JSON.parse(s)
来源：http://tss.jinqigufen.top

TS:   JSON.parse(s)
来源：http://tsq.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mck.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://dvl.fktsv.cn

Ruby: JSON.parse(s)
来源：http://khp.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://plb.ywan-chungtsiang.top

[K03] JSON 美化输出（带缩进）
来源：http://frf.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nsp.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dnm.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mls.xuanzx.com

TS:   JSON.stringify(obj, null, 2)
来源：http://lkj.jyoumei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fxl.meibo888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iws.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://may.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dhs.yfazqb.com

[K04] 读取 JSON 文件
来源：http://ist.jyoumei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dmd.0kj1m.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ffy.shanyushiyangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iyr.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hgs.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wod.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xfv.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://bma.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://btu.yongpay.top

[K05] 深拷贝对象
来源：http://duv.svipenyu.cn

Py:   copy.deepcopy(obj)
来源：http://pil.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://sba.hnxiangtu.top

JS:   structuredClone(obj)
来源：http://cwf.chenlongwang.top

TS:   structuredClone(obj)
来源：http://hnq.haohaochexian.top

Java: // 手写拷贝构造，或序列化往返
来源：http://krh.zhongyouzk.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://erv.fengsongda.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yrh.sxryk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://roa.bjfxy.top

[K06] 解析 URL 查询串
来源：http://evi.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rcz.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rlt.hnqzz.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://voj.chenlongwang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pej.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wka.quarkkingdee.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mul.xziqi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hqu.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mnf.cqqwz.cn

[K07] 进制转换
来源：http://wgr.nwbrower.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mve.cdnleiting.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xnd.ivvv.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nll.cucudq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ycc.jinqigfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://djf.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://icp.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vtu.zycfv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cbw.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://pac.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://wzk.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://tan.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://rjc.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://qqr.ywan-chungtsiang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://grt.guowangkeji.top

Go:   encoding/gob
来源：http://gjn.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://vvv.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zct.chenjidiqi.icu

================================================================================
来源：http://ywr.52xcode.cn

L. 网络请求
来源：http://tyk.snrcjt.cn

================================================================================
来源：http://jmn.gogol.net.cn

[L01] 发送 GET 请求
来源：http://qsr.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bth.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://muw.dashuyun.cn

JS:   await fetch(url)
来源：http://fkn.yuanzhike.top

TS:   await fetch(url)
来源：http://zvm.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cbh.hysaishi.cn

Go:   resp, err := http.Get(url)
来源：http://vom.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://has.shzxlz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mjr.cheryme.top

[L02] 发送 POST JSON
来源：http://zhy.nanxuanxn.top

Py:   requests.post(url, json={"a": 1})
来源：http://oqg.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nqt.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jsx.hysaishi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iul.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jkl.smart0.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bfz.kuanghao11.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hcr.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qbj.sweek.top

[L03] 设置自定义请求头
来源：http://xtw.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wks.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cbp.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ohb.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rop.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yfp.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ttn.hcnkem.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bqf.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xlo.ybcxt.top

[L04] 设置超时
来源：http://sfd.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://swv.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rum.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xad.zhiwuduotai.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ene.xuanzx.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iuk.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://moh.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ooh.yongpay.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://slg.smart0.xyz

[L05] 上传文件（multipart）
来源：http://qtl.wangdashe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mvm.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vor.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://riz.sufxvd.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nyi.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lgq.fanxiaobao.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pmy.tanke756.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cqb.yueranfly.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://foa.snrcjt.cn

[L06] 解析响应为 JSON
来源：http://vkh.cheryme.top

Py:   resp.json()
来源：http://fzu.ybcxt.top

PHP:  json_decode($body, true);
来源：http://zcd.zhijiandao.cn

JS:   await resp.json()
来源：http://eun.zhixingplan.top

TS:   await resp.json()
来源：http://vvx.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nje.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gxq.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://boe.cucudq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://scz.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://gnw.fktsv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bua.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uju.52xcode.cn

JS:   resp.ok;  resp.status
来源：http://gvs.yj202588.top

TS:   resp.ok;  resp.status
来源：http://xua.gotoacloud.top

Java: resp.statusCode()
来源：http://rlv.xziqi.cn

Go:   resp.StatusCode
来源：http://ttq.yangfankeji.com

Ruby: resp.code.to_i
来源：http://ctp.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://jwl.andypj.xyz

[L08] 并发请求多个地址
来源：http://sts.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dti.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://bjn.vehdjk.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oom.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://svd.fanxiaobao.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eea.vqdsnc.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qrc.shuidangran.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tcw.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sfa.9152youxi.cn

================================================================================
来源：http://hdh.tarul.cn

M. 命令行 / 进程 / 环境
来源：http://itc.sxryk.cn

================================================================================
来源：http://taa.zhijiandao.cn

[M01] 读取命令行参数
来源：http://ehw.zycfv.cn

Py:   sys.argv[1:]
来源：http://uou.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://ppo.0kj1m.cn

JS:   process.argv.slice(2)
来源：http://zyh.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://snj.fehbvm.com

Java: args 数组（main 方法参数）
来源：http://tdh.zycfv.cn

Go:   os.Args[1:]
来源：http://cgp.9152youxi.cn

Ruby: ARGV
来源：http://pgy.chenlongwang.top

C#:   args 数组（Main 方法参数）
来源：http://dyc.smart0.xyz

[M02] 读取环境变量
来源：http://tru.dashuyun.cn

Py:   os.environ.get("HOME")
来源：http://evm.ctjpmb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ryw.hfpthk.cn

JS:   process.env.HOME
来源：http://uvi.ywan-chungtsiang.top

TS:   process.env.HOME
来源：http://hrj.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://sun.jinqigfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ffa.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://qvf.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ukz.shangyingyoupin.top

[M03] 执行外部命令
来源：http://len.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iep.jyoumei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://llq.andypj.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://keq.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nma.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hji.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pxe.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://phb.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://bwz.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://jdc.yj20258.top

Py:   os.getcwd()
来源：http://mks.fzhhl.top

PHP:  getcwd();
来源：http://qad.zhengqikj.top

JS:   process.cwd()
来源：http://anw.tarul.cn

TS:   process.cwd()
来源：http://kpi.sweek.top

Java: Path.of("").toAbsolutePath()
来源：http://emp.tanke756.top

Go:   os.Getwd()
来源：http://ysa.hesvh.cn

Ruby: Dir.pwd
来源：http://oor.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://cpr.shuidangran.top

[M05] 设置退出码
来源：http://xvy.shanyushiyangtech.top

Py:   sys.exit(1)
来源：http://sbn.chenzaomai.com

PHP:  exit(1);
来源：http://peq.hnqzz.top

JS:   process.exit(1)
来源：http://kle.redwolf501.top

TS:   process.exit(1)
来源：http://nll.uphjek.com

Java: System.exit(1)
来源：http://rfs.snrcjt.cn

Go:   os.Exit(1)
来源：http://ryz.feifeiyinyue.top

Ruby: exit 1
来源：http://thw.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rbw.xylfe.cn

[M06] 向标准错误输出
来源：http://xjy.chenzaomai.com

Py:   print("err", file=sys.stderr)
来源：http://taq.jianghu66.top

PHP:  fwrite(STDERR, "err\n");
来源：http://krv.sweek.top

JS:   console.error("err")
来源：http://rpr.yj20258888.top

TS:   console.error("err")
来源：http://nae.andypj.xyz

Java: System.err.println("err")
来源：http://bac.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uls.jyoumei.cn

Ruby: warn "err"
来源：http://nrp.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://obo.fehbvm.com

[M07] 判断是否为主入口
来源：http://bpc.9152youxi.cn

Py:   if __name__ == "__main__":
来源：http://efn.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://clp.hnxiangtu.top

JS:   require.main === module
来源：http://fxx.pycfn.com

TS:   require.main === module
来源：http://ovr.jianghu66.top

Java: public static void main(String[] args)
来源：http://ytk.0kj1m.cn

Go:   func main()
来源：http://usx.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yav.tanke756.top

C#:   static void Main(string[] args)
来源：http://avn.nanxuanxn.top

[M08] 获取系统与运行时信息
来源：http://uci.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://frp.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://fsy.vehdjk.com

JS:   process.platform;  process.version
来源：http://flr.sufxvd.cn

TS:   process.platform;  process.version
来源：http://hrl.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hnp.havefunace.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xal.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ede.fktsv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vwk.yanxiufei.cn

================================================================================
来源：http://txd.epnwcf.com

N. 数据结构与算法
来源：http://isa.chenlongwang.top

================================================================================
来源：http://bkj.zdbjq.cn

[N01] 二分查找（有序数组）
来源：http://maw.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cbh.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ypr.sufxvd.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qfb.fehbvm.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qzn.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://dey.0kj1m.cn

Go:   sort.SearchInts(arr, x)
来源：http://jps.snrcjt.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rzf.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://adp.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://lvq.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://afs.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dwh.hammf.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://eyd.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jgv.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://deq.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://esx.fengsongda.top

Ruby: arr.sort
来源：http://nde.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vvk.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://oqr.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zwe.jqgfzy.top

PHP:  // 递归实现，或用 usort
来源：http://usk.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kce.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://itv.yfazqb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ifx.jiagoushi.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://beb.yanxiufei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zyc.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://oho.vehdjk.com

[N04] 斐波那契数列
来源：http://vpb.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eov.xylfe.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nhf.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://als.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://prr.yanxiufei.cn


<!-- 参考信息 -->