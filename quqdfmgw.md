代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://ptx.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://kiu.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://tlu.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://iza.ctjpmb.com

[J07] 比较两个日期
来源：http://jhb.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://caz.wangdashe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iez.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://pyl.tianlin.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://njq.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xob.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yda.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://iek.jianghu66.top

C#:   d1 < d2;  d1 == d2
来源：http://vcm.chenjidiqi.icu

[J08] 提取年月日与星期
来源：http://piv.chenzaomai.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xax.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vsu.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://shh.jinqigufen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wct.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vxm.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lyr.birdmap.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hml.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bhn.epnwcf.com

[J09] 时区处理
来源：http://yve.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uzg.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jch.kuanghao11.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ynl.jlsjyb.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dwi.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qyi.bbcook.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jdv.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://mtz.cheryme.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jou.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://pnz.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kgk.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xys.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rnp.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wwt.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hzt.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hnx.gogol.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ipz.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://clx.vehdjk.com

================================================================================
来源：http://gkx.vehdjk.com

K. JSON 与序列化
来源：http://lvx.nanxuanxn.top

================================================================================
来源：http://nid.xylfe.cn

[K01] 对象转 JSON 字符串
来源：http://esb.iojbl.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sab.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lxo.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://zdb.shzxlz.cn

TS:   JSON.stringify(obj)
来源：http://lwi.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qcj.yj20258888.top

Go:   json.Marshal(obj)
来源：http://doo.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://dht.smart0.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://goc.yj20258888.top

[K02] JSON 字符串转对象
来源：http://iqc.jqgufenzy.top

Py:   json.loads(s)
来源：http://iwb.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wqe.ctjpmb.com

JS:   JSON.parse(s)
来源：http://daf.xinyue.icu

TS:   JSON.parse(s)
来源：http://jvs.hywenlv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lrr.wangshuangyany.cn

Go:   json.Unmarshal(data, &v)
来源：http://hgy.52xcode.cn

Ruby: JSON.parse(s)
来源：http://ehe.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uwt.svipenyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://rth.hywenlv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jaf.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fmr.tarul.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zel.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://asa.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wal.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qla.bbcook.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jxm.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pev.xylfe.cn

[K04] 读取 JSON 文件
来源：http://mxl.hesvh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mlb.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tos.zycfv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hjl.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cpq.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://seb.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hcp.shuidangran.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yrb.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qxb.yuxming.cn

[K05] 深拷贝对象
来源：http://dmk.zhixingplan.top

Py:   copy.deepcopy(obj)
来源：http://exn.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://vgj.wangdashe.top

JS:   structuredClone(obj)
来源：http://qtl.hysaishi.cn

TS:   structuredClone(obj)
来源：http://srg.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bod.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cpu.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pxs.fzhhl.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qrd.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://rat.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oxy.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://thn.hcnkem.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ooy.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://asm.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lsg.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://iwx.sufxvd.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nph.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ban.gaohongyu789.top

[K07] 进制转换
来源：http://hqm.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jzk.shanyushiyangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hut.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://avz.hesvh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sse.chenlongwang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zzm.xuetiantiany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aku.wangshuangyany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yoc.pycfn.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kqw.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://cuh.shuidangran.top

Py:   pickle.dumps(obj)
来源：http://wvz.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pbj.52xcode.cn

JS:   v8.serialize(obj)        // Node
来源：http://crn.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://ejt.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nza.fktsv.cn

Go:   encoding/gob
来源：http://idi.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://hfb.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rxz.ydzc1.top

================================================================================
来源：http://mfq.fanxiaobao.xyz

L. 网络请求
来源：http://cuf.zhoulong.xyz

================================================================================
来源：http://igj.nwbrower.top

[L01] 发送 GET 请求
来源：http://etx.daxiang520.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yro.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xab.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://pzw.havefunace.top

TS:   await fetch(url)
来源：http://yyp.jianghu66.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ioq.chenzaomai.com

Go:   resp, err := http.Get(url)
来源：http://jsv.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://egx.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lcv.wangdashe.top

[L02] 发送 POST JSON
来源：http://pbf.ywan-chungtsiang.top

Py:   requests.post(url, json={"a": 1})
来源：http://tzi.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xtw.gaohongyu789.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ydg.xziqi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://son.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qhz.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xbe.yvedp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rtn.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pvj.chenlongwang.top

[L03] 设置自定义请求头
来源：http://ucx.wangshuangyany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dhy.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tpv.uphjek.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fbc.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oiz.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bsf.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pvv.daxiang520.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yps.cheryme.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uet.vqdsnc.cn

[L04] 设置超时
来源：http://xjx.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://xpb.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xfy.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oov.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ezs.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qeo.xingfuxueyuan.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pav.yvedp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cts.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gat.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://evo.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gov.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yid.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xyq.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aqr.zhixingplan.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pzf.redwolf501.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qgi.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://txo.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rko.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://lwr.jqgufenzy.top

Py:   resp.json()
来源：http://qam.ydzc1.top

PHP:  json_decode($body, true);
来源：http://end.zhijiandao.cn

JS:   await resp.json()
来源：http://vme.mhx1999.top

TS:   await resp.json()
来源：http://bgn.zhixingplan.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tyc.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lkd.guowangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://wsm.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pay.chenzaomai.com

[L07] 处理 HTTP 状态码
来源：http://wet.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eha.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fkf.wangdashe.top

JS:   resp.ok;  resp.status
来源：http://fgf.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://ikq.cheryme.top

Java: resp.statusCode()
来源：http://uqd.guowangkeji.top

Go:   resp.StatusCode
来源：http://usv.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://jlk.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://vbm.hfpthk.cn

[L08] 并发请求多个地址
来源：http://chs.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xou.daria6918.cn

PHP:  curl_multi_init() 系列
来源：http://psm.hnxiangtu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qaz.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tku.ivvv.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://emb.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://juw.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://apm.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gdd.sweek.top

================================================================================
来源：http://wmw.sufxvd.cn

M. 命令行 / 进程 / 环境
来源：http://vrm.chenjidiqi.icu

================================================================================
来源：http://kse.gotoacloud.top

[M01] 读取命令行参数
来源：http://ify.cdnleiting.top

Py:   sys.argv[1:]
来源：http://eql.yueranfly.top

PHP:  $argv;  $argc;
来源：http://vsf.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://utz.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://wjr.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://awf.c1oappe.top

Go:   os.Args[1:]
来源：http://ghz.hammf.cn

Ruby: ARGV
来源：http://jcq.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://ofh.ctjpmb.com

[M02] 读取环境变量
来源：http://xwv.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://pbd.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pth.fehbvm.com

JS:   process.env.HOME
来源：http://eww.pengpengdd.cyou

TS:   process.env.HOME
来源：http://vyp.ehwqpu.com

Java: System.getenv("HOME")
来源：http://gzf.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bqu.hesvh.cn

Ruby: ENV["HOME"]
来源：http://qgn.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nbi.cashguo.top

[M03] 执行外部命令
来源：http://wgj.aizwys.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cyl.ydjk.org.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bma.ppjwa.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rmj.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cvx.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bru.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zyr.chenjidiqi.icu

Ruby: system("ls -l");  `ls -l`
来源：http://rgl.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://ngy.cqqwz.cn

[M04] 获取当前工作目录
来源：http://obz.birdmap.top

Py:   os.getcwd()
来源：http://qmi.hongshengwenyu.top

PHP:  getcwd();
来源：http://cez.sufxvd.cn

JS:   process.cwd()
来源：http://exx.jqgfzy.top

TS:   process.cwd()
来源：http://jjk.yangfankeji.com

Java: Path.of("").toAbsolutePath()
来源：http://mey.chenzaomai.com

Go:   os.Getwd()
来源：http://nnp.pycfn.com

Ruby: Dir.pwd
来源：http://zpl.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zuq.yfazqb.com

[M05] 设置退出码
来源：http://plg.hcnkem.com

Py:   sys.exit(1)
来源：http://zpy.shanyushiyangtech.top

PHP:  exit(1);
来源：http://ztb.aibaodan.cn

JS:   process.exit(1)
来源：http://wdz.vqdsnc.cn

TS:   process.exit(1)
来源：http://nck.nanxuanxn.top

Java: System.exit(1)
来源：http://thw.nwbrower.top

Go:   os.Exit(1)
来源：http://ydd.hongshengwenyu.top

Ruby: exit 1
来源：http://vlt.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uos.birdmap.top

[M06] 向标准错误输出
来源：http://gnz.sweek.top

Py:   print("err", file=sys.stderr)
来源：http://pjt.guannengcc.top

PHP:  fwrite(STDERR, "err\n");
来源：http://stn.jlsjyb.cn

JS:   console.error("err")
来源：http://bra.jinyuanbaomall.cn

TS:   console.error("err")
来源：http://tkk.tanke756.top

Java: System.err.println("err")
来源：http://hre.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ukm.daria6918.cn

Ruby: warn "err"
来源：http://str.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://vkt.zdqjudy.top

[M07] 判断是否为主入口
来源：http://idd.feifeiyinyue.top

Py:   if __name__ == "__main__":
来源：http://cgx.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zty.dianchejie.cn

JS:   require.main === module
来源：http://dse.ybcxt.top

TS:   require.main === module
来源：http://bnv.ehwqpu.com

Java: public static void main(String[] args)
来源：http://aks.xuetiantiany.cn

Go:   func main()
来源：http://icm.fktsv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://apy.gaohongyu789.top

C#:   static void Main(string[] args)
来源：http://nih.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://cqh.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://ccl.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://xjz.cqqwz.cn

JS:   process.platform;  process.version
来源：http://awz.meibo888.top

TS:   process.platform;  process.version
来源：http://pvy.cqqwz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hll.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://iah.hnxiangtu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xvk.jinghuilouyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nfu.zhiwuduotai.top

================================================================================
来源：http://tct.sufxvd.cn

N. 数据结构与算法
来源：http://doo.zhiwuduotai.top

================================================================================
来源：http://his.jiagoushi.top

[N01] 二分查找（有序数组）
来源：http://qzk.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://nhm.zdqjudy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jfj.xuetiantiany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://skz.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rgi.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vdi.guowangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://ygm.vehdjk.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://tha.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://jjs.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://hiy.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://ppp.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fpj.iojbl.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wmu.tianlin.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://yey.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jri.jinyuanbaomall.cn

Go:   slices.Sort(arr)
来源：http://cdo.jinghuilouyu.cn

Ruby: arr.sort
来源：http://hbi.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mqt.hfpthk.cn

[N03] 快速排序（分治示例）
来源：http://zdl.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rgw.havefunace.top

PHP:  // 递归实现，或用 usort
来源：http://uiu.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ysp.chenzaomai.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://upb.hammf.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ltw.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ewl.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rdc.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://bwy.jqgfzy.top

[N04] 斐波那契数列
来源：http://xfc.zhiwuduotai.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lkp.yfazqb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kzs.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://boc.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ipq.zhengqikj.top


<!-- 参考信息 -->