代发 wailian999

Py:   (end - start).total_seconds()
来源：http://koj.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://htq.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bdp.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zoz.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://lmg.jinqigufen.top

Go:   end.Sub(start).Hours()
来源：http://omk.redwolf501.top

Ruby: end - start                 # 返回秒数
来源：http://soe.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://ehd.svipenyu.cn

[J07] 比较两个日期
来源：http://qad.cashguo.top

Py:   d1 < d2;  d1 == d2
来源：http://gvw.xziqi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vof.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://evk.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kei.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bht.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bja.zhijiandao.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cax.dashuyun.cn

C#:   d1 < d2;  d1 == d2
来源：http://tgo.yonumen.top

[J08] 提取年月日与星期
来源：http://cel.aizwys.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vlt.jinqigufen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hib.yongpay.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ous.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qft.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sxx.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qil.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qbs.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://psg.zdbjq.cn

[J09] 时区处理
来源：http://dak.ywan-chungtsiang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kau.jyoumei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blt.vehdjk.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ybg.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://szu.jlsjyb.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mbj.gogol.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gze.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sbu.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://frj.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://jli.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fef.tanke756.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dep.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://erv.nanxuanxn.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://acb.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iyx.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qkn.shangyingyoupin.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ghj.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://odl.andypj.xyz

================================================================================
来源：http://ach.vqdsnc.cn

K. JSON 与序列化
来源：http://phc.xziqi.cn

================================================================================
来源：http://xjv.yuanzhike.top

[K01] 对象转 JSON 字符串
来源：http://egk.hywenlv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://efd.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qlm.bbcook.cn

JS:   JSON.stringify(obj)
来源：http://uqq.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://aya.zhongyouzk.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uac.gotoacloud.top

Go:   json.Marshal(obj)
来源：http://uij.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://vds.ybcxt.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kyk.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://vfr.dianchejie.cn

Py:   json.loads(s)
来源：http://kge.hnqzz.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bzc.jiagoushi.top

JS:   JSON.parse(s)
来源：http://fim.gogol.net.cn

TS:   JSON.parse(s)
来源：http://tcd.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fev.chenjidiqi.icu

Go:   json.Unmarshal(data, &v)
来源：http://hvq.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://xuu.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ozx.yj202588.top

[K03] JSON 美化输出（带缩进）
来源：http://xri.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fxm.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ace.xinyue.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://laa.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dxi.zhongyouzk.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://izw.shzxlz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dxa.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://klm.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wmn.c1oappe.top

[K04] 读取 JSON 文件
来源：http://vrm.xinyue.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lbi.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ybc.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tyu.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jsn.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fpc.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dif.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lzy.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gyv.bjfxy.top

[K05] 深拷贝对象
来源：http://rte.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://qfy.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://xbn.kuanghao11.cn

JS:   structuredClone(obj)
来源：http://jwq.guowangkeji.top

TS:   structuredClone(obj)
来源：http://yov.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oqy.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nua.xuetiantiany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rwa.hnqzz.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nnq.guannengcc.top

[K06] 解析 URL 查询串
来源：http://wpy.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://guz.0kj1m.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hwj.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wug.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sil.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ylh.xuetiantiany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wjf.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vfq.chenzaomai.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nnd.nwbrower.top

[K07] 进制转换
来源：http://roh.shuidangran.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://erl.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://npw.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eqa.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wau.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jvj.tarul.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gar.hesvh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gzk.jiagoushi.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fbu.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://wtk.zhaomingkeji.xyz

Py:   pickle.dumps(obj)
来源：http://dfn.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fre.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://vki.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://fxo.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yfm.fanxiaobao.xyz

Go:   encoding/gob
来源：http://ccm.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://hln.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tjn.yj20258888.top

================================================================================
来源：http://lzj.zhongyouzk.top

L. 网络请求
来源：http://qdo.sjlbkw.cn

================================================================================
来源：http://fhy.gzhubu.top

[L01] 发送 GET 请求
来源：http://meu.ydzc1.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wyp.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jyd.sjlbkw.cn

JS:   await fetch(url)
来源：http://yqg.zhoulong.xyz

TS:   await fetch(url)
来源：http://xiu.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xpm.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://ele.iojbl.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yib.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zfj.chenjidiqi.icu

[L02] 发送 POST JSON
来源：http://cly.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://jcg.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hah.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mbf.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://btp.yongpay.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hxu.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vuo.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mpp.cdnleiting.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xpd.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://zzi.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wfr.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qyw.shanyushiyangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zjn.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://emq.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ilo.yj20258.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://riq.hnxiangtu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://axm.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lli.xylfe.cn

[L04] 设置超时
来源：http://xpe.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://sti.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pff.jqgfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cie.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fro.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mfn.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dic.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mzx.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iog.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://cpk.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://asu.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nxu.snrcjt.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://njl.tianlin.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iyd.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wzv.andypj.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cyk.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dvk.kuanghao11.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://owi.zycfv.cn

[L06] 解析响应为 JSON
来源：http://beh.shangyingyoupin.top

Py:   resp.json()
来源：http://nex.xuanzx.com

PHP:  json_decode($body, true);
来源：http://nim.cheryme.top

JS:   await resp.json()
来源：http://haa.sjlbkw.cn

TS:   await resp.json()
来源：http://pts.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jqf.andypj.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eei.ctjpmb.com

Ruby: JSON.parse(resp.body)
来源：http://pqt.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rch.chenlongwang.top

[L07] 处理 HTTP 状态码
来源：http://whn.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://prj.xingfuxueyuan.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jvy.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://gms.iojbl.cn

TS:   resp.ok;  resp.status
来源：http://gpg.gogol.net.cn

Java: resp.statusCode()
来源：http://kwm.sweek.top

Go:   resp.StatusCode
来源：http://hkg.yongpay.top

Ruby: resp.code.to_i
来源：http://rge.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://ops.zhixingplan.top

[L08] 并发请求多个地址
来源：http://ynm.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mzk.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://tjl.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jct.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hdp.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qbm.ywan-chungtsiang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ngx.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iqm.ybcxt.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://snf.xingfuxueyuan.xyz

================================================================================
来源：http://mcp.redwolf501.top

M. 命令行 / 进程 / 环境
来源：http://ppi.guowangkeji.top

================================================================================
来源：http://gss.svipenyu.cn

[M01] 读取命令行参数
来源：http://bys.guowangkeji.top

Py:   sys.argv[1:]
来源：http://cqw.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://wkt.xinyue.icu

JS:   process.argv.slice(2)
来源：http://nqk.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://yft.xziqi.cn

Java: args 数组（main 方法参数）
来源：http://vsg.yanxiufei.cn

Go:   os.Args[1:]
来源：http://tfi.nwbrower.top

Ruby: ARGV
来源：http://rac.hongshengwenyu.top

C#:   args 数组（Main 方法参数）
来源：http://iax.zdbjq.cn

[M02] 读取环境变量
来源：http://jqy.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://klt.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cxe.sweek.top

JS:   process.env.HOME
来源：http://jwi.ehwqpu.com

TS:   process.env.HOME
来源：http://eqg.hnxiangtu.top

Java: System.getenv("HOME")
来源：http://zhx.nanxinkj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yqw.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://ihr.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wsv.cheryme.top

[M03] 执行外部命令
来源：http://kln.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vob.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://swm.wangdashe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://odo.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qhy.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aoy.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mil.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://azv.hysaishi.cn

C#:   Process.Start("ls", "-l");
来源：http://ffr.yuanzhike.top

[M04] 获取当前工作目录
来源：http://umf.wangdashe.top

Py:   os.getcwd()
来源：http://ndj.bjfxy.top

PHP:  getcwd();
来源：http://ysr.zdbjq.cn

JS:   process.cwd()
来源：http://gye.wangdashe.top

TS:   process.cwd()
来源：http://stq.yangfankeji.com

Java: Path.of("").toAbsolutePath()
来源：http://cys.hongshengwenyu.top

Go:   os.Getwd()
来源：http://qls.nanxinkj.top

Ruby: Dir.pwd
来源：http://aer.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://osm.wangshuangyany.cn

[M05] 设置退出码
来源：http://euw.sxryk.cn

Py:   sys.exit(1)
来源：http://rny.hnqzz.top

PHP:  exit(1);
来源：http://vxz.meibo888.top

JS:   process.exit(1)
来源：http://ner.sweek.top

TS:   process.exit(1)
来源：http://scj.andypj.xyz

Java: System.exit(1)
来源：http://sle.jqgfzy.top

Go:   os.Exit(1)
来源：http://uai.meibo888.top

Ruby: exit 1
来源：http://uou.yuxming.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zjf.zhengqikj.top

[M06] 向标准错误输出
来源：http://qqh.nwbrower.top

Py:   print("err", file=sys.stderr)
来源：http://rwg.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ohr.uphjek.com

JS:   console.error("err")
来源：http://bjh.hnxiangtu.top

TS:   console.error("err")
来源：http://ggv.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://utx.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gbk.redwolf501.top

Ruby: warn "err"
来源：http://dar.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://pdq.epnwcf.com

[M07] 判断是否为主入口
来源：http://liw.cqqwz.cn

Py:   if __name__ == "__main__":
来源：http://rzh.nanxuanxn.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hug.epnwcf.com

JS:   require.main === module
来源：http://jdy.ehwqpu.com

TS:   require.main === module
来源：http://uml.sysykeji.top

Java: public static void main(String[] args)
来源：http://tdf.ydzc1.top

Go:   func main()
来源：http://zfa.nwbrower.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kqr.jqgfzy.top

C#:   static void Main(string[] args)
来源：http://bhj.yonumen.top

[M08] 获取系统与运行时信息
来源：http://bod.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://nif.hywenlv.cn

PHP:  PHP_OS;  phpversion();
来源：http://cez.gotoacloud.top

JS:   process.platform;  process.version
来源：http://bxn.ppjwa.cn

TS:   process.platform;  process.version
来源：http://icf.zhongyouzk.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://piu.epnwcf.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://bww.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ngm.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://glu.9152youxi.cn

================================================================================
来源：http://grv.jlsjyb.cn

N. 数据结构与算法
来源：http://loq.uphjek.com

================================================================================
来源：http://kxw.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://iqw.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wzg.daxiang520.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qdg.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://djk.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dmo.aibaodan.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lmm.smart0.xyz

Go:   sort.SearchInts(arr, x)
来源：http://cqy.zhijiandao.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tvd.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://awf.yuxming.cn

[N02] 排序（工程实践用内置实现）
来源：http://fih.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://wko.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ekn.nanxuanxn.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rfq.jqgfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ojk.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://egc.cashguo.top

Go:   slices.Sort(arr)
来源：http://irl.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://hfy.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ecc.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://ptv.jinqigfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ald.nanxuanxn.top

PHP:  // 递归实现，或用 usort
来源：http://dzs.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hgt.meibo888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://duj.gogol.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ztu.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jyt.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jli.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://fsf.sufxvd.cn

[N04] 斐波那契数列
来源：http://hva.dashuyun.cn


<!-- 参考信息 -->