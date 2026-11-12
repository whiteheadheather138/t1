代发 wailian999

[J07] 比较两个日期
来源：http://kvc.tianlin.xyz

Py:   d1 < d2;  d1 == d2
来源：http://vwh.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eqh.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yom.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://flw.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yxt.hysaishi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yqa.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://lkx.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://hhj.birdmap.top

[J08] 提取年月日与星期
来源：http://qhp.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qez.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ljn.zdqjudy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yee.svipenyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aza.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pcg.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vel.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eek.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://elu.guowangkeji.top

[J09] 时区处理
来源：http://xwj.aizwys.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kmj.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rmp.zhoulong.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://svn.0kj1m.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iel.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qsf.fktsv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jll.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hhq.chenjidiqi.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jqo.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://abz.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jtu.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nfp.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ysp.jyoumei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iob.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gvi.yongpay.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uma.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bvg.chenlongwang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wxd.jqgufenzy.top

================================================================================
来源：http://wfy.hnqzz.top

K. JSON 与序列化
来源：http://iqe.xingfuxueyuan.xyz

================================================================================
来源：http://vox.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://erc.hnqzz.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rqo.yuxming.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ijt.bbcook.cn

JS:   JSON.stringify(obj)
来源：http://vbb.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://wkt.tian-w.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cit.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://hed.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://yek.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://nju.aizwys.cn

[K02] JSON 字符串转对象
来源：http://hxi.hcnkem.com

Py:   json.loads(s)
来源：http://apw.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uog.jinqigufen.top

JS:   JSON.parse(s)
来源：http://ktu.nanxuanxn.top

TS:   JSON.parse(s)
来源：http://ldp.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ewc.xziqi.cn

Go:   json.Unmarshal(data, &v)
来源：http://jdz.sjlbkw.cn

Ruby: JSON.parse(s)
来源：http://pen.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tzw.hesvh.cn

[K03] JSON 美化输出（带缩进）
来源：http://uwc.chenjidiqi.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hqi.tanke756.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pxd.hesvh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jmc.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vkh.bbcook.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lwk.jinghuilouyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ule.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://poe.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kra.hywenlv.cn

[K04] 读取 JSON 文件
来源：http://ugt.hnxiangtu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gck.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xjf.nanxuanxn.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mfx.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zvj.jinqigufen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tgt.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xra.ydzc1.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ipl.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hpw.xziqi.cn

[K05] 深拷贝对象
来源：http://wum.tarul.cn

Py:   copy.deepcopy(obj)
来源：http://lzd.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://nos.yangfankeji.com

JS:   structuredClone(obj)
来源：http://slk.tanke756.top

TS:   structuredClone(obj)
来源：http://qsf.hnqzz.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bcm.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qjz.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jbj.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://mux.yj20258888.top

[K06] 解析 URL 查询串
来源：http://bvp.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ylo.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qxy.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aaf.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zqj.yonumen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://trl.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wza.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vhm.jqgfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zzh.shangyingyoupin.top

[K07] 进制转换
来源：http://cus.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ksi.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vhp.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uwk.ydzc1.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://deh.tianlin.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gxb.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uco.hfpthk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rwn.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eaz.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://uup.jinyuanbaomall.cn

Py:   pickle.dumps(obj)
来源：http://dbt.vqdsnc.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ajd.guowangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://qds.bbcook.cn

TS:   v8.serialize(obj)        // Node
来源：http://xdo.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yju.wangshuangyany.cn

Go:   encoding/gob
来源：http://cqv.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://gbg.hammf.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://upw.zdqjudy.top

================================================================================
来源：http://iri.havefunace.top

L. 网络请求
来源：http://rzh.uphjek.com

================================================================================
来源：http://cyi.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://qnv.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://abz.birdmap.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zyw.hcnkem.com

JS:   await fetch(url)
来源：http://oce.jiagoushi.top

TS:   await fetch(url)
来源：http://juk.vehdjk.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qwi.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://vax.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nkx.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wyh.havefunace.top

[L02] 发送 POST JSON
来源：http://idb.yfazqb.com

Py:   requests.post(url, json={"a": 1})
来源：http://xys.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cpe.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tcp.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bst.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pse.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pkm.xinyue.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sub.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nfw.zhixingplan.top

[L03] 设置自定义请求头
来源：http://wuy.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sct.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hcv.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lwe.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nqn.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ipc.guowangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kdz.sweek.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://len.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dtu.52xcode.cn

[L04] 设置超时
来源：http://knn.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://njn.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hkt.nanxuanxn.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fjk.zhongyouzk.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://epp.tarul.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ccr.yuanzhike.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yln.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bjt.gaohongyu789.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qfp.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://kzi.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ghk.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nnw.quarkkingdee.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://knd.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ffk.daria6918.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iuj.tian-w.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://phf.zycfv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qpa.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pxp.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://uzj.jinqigufen.top

Py:   resp.json()
来源：http://juq.fehbvm.com

PHP:  json_decode($body, true);
来源：http://nty.shanyushiyangkeji.top

JS:   await resp.json()
来源：http://pve.yvedp.cn

TS:   await resp.json()
来源：http://nwm.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cxw.tian-w.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tjn.316326.xyz

Ruby: JSON.parse(resp.body)
来源：http://jnd.cashguo.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pxy.quarkkingdee.top

[L07] 处理 HTTP 状态码
来源：http://zyp.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pnk.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lxx.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://mpi.hongshengwenyu.top

TS:   resp.ok;  resp.status
来源：http://vix.chenlongwang.top

Java: resp.statusCode()
来源：http://idi.hfpthk.cn

Go:   resp.StatusCode
来源：http://eld.ywan-chungtsiang.top

Ruby: resp.code.to_i
来源：http://ruj.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://bnb.yuxming.cn

[L08] 并发请求多个地址
来源：http://gee.havefunace.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://grg.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://ebt.yangfankeji.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://unr.aibaodan.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hdz.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://brb.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nmg.sufxvd.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hti.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://szg.jinyuanbaomall.cn

================================================================================
来源：http://agl.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://xex.chenlongwang.top

================================================================================
来源：http://bvl.wangdashe.top

[M01] 读取命令行参数
来源：http://esy.redwolf501.top

Py:   sys.argv[1:]
来源：http://awg.sysykeji.top

PHP:  $argv;  $argc;
来源：http://wii.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://pew.shzxlz.cn

TS:   process.argv.slice(2)
来源：http://huw.svipenyu.cn

Java: args 数组（main 方法参数）
来源：http://jft.hcnkem.com

Go:   os.Args[1:]
来源：http://oxx.fehbvm.com

Ruby: ARGV
来源：http://ubo.pengpengdd.cyou

C#:   args 数组（Main 方法参数）
来源：http://efo.uphjek.com

[M02] 读取环境变量
来源：http://hel.chenlongwang.top

Py:   os.environ.get("HOME")
来源：http://bew.fengsongda.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://olq.feifeiyinyue.top

JS:   process.env.HOME
来源：http://lfg.fehbvm.com

TS:   process.env.HOME
来源：http://zcz.cdnleiting.top

Java: System.getenv("HOME")
来源：http://evq.fktsv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://thv.ybcxt.top

Ruby: ENV["HOME"]
来源：http://vbq.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ukb.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://epg.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qjn.zycfv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://evg.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://qnj.hongshengwenyu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zfj.sufxvd.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zrz.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://axh.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://clo.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://fiu.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://iva.hongshengwenyu.top

Py:   os.getcwd()
来源：http://jbr.ctjpmb.com

PHP:  getcwd();
来源：http://ite.aizwys.cn

JS:   process.cwd()
来源：http://uvf.bbcook.cn

TS:   process.cwd()
来源：http://vnp.sweek.top

Java: Path.of("").toAbsolutePath()
来源：http://jre.yongpay.top

Go:   os.Getwd()
来源：http://gst.tanke756.top

Ruby: Dir.pwd
来源：http://clj.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://yjv.nanxinkj.top

[M05] 设置退出码
来源：http://fxg.fzhhl.top

Py:   sys.exit(1)
来源：http://klc.cheryme.top

PHP:  exit(1);
来源：http://smd.cheryme.top

JS:   process.exit(1)
来源：http://ylg.yangfankeji.com

TS:   process.exit(1)
来源：http://zja.jlsjyb.cn

Java: System.exit(1)
来源：http://vds.zhijiandao.cn

Go:   os.Exit(1)
来源：http://sll.ydjk.org.cn

Ruby: exit 1
来源：http://sop.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gws.shzxlz.cn

[M06] 向标准错误输出
来源：http://tpw.fktsv.cn

Py:   print("err", file=sys.stderr)
来源：http://clm.hammf.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dat.fengsongda.top

JS:   console.error("err")
来源：http://yqh.zhengqikj.top

TS:   console.error("err")
来源：http://zel.zdqjudy.top

Java: System.err.println("err")
来源：http://awf.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oin.0kj1m.cn

Ruby: warn "err"
来源：http://osa.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://gkm.jinqigufen.top

[M07] 判断是否为主入口
来源：http://taj.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://ehf.316326.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ehx.zdbjq.cn

JS:   require.main === module
来源：http://uad.yfazqb.com

TS:   require.main === module
来源：http://yey.ybcxt.top

Java: public static void main(String[] args)
来源：http://uix.chenlongwang.top

Go:   func main()
来源：http://lkm.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sgg.xuetiantiany.cn

C#:   static void Main(string[] args)
来源：http://wpe.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://ukv.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://ovq.zycfv.cn

PHP:  PHP_OS;  phpversion();
来源：http://swi.ybcxt.top

JS:   process.platform;  process.version
来源：http://yxr.fktsv.cn

TS:   process.platform;  process.version
来源：http://xlt.fktsv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yov.kuanghao11.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://opr.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jzf.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qaa.cdnleiting.top

================================================================================
来源：http://mzd.jinghuilouyu.cn

N. 数据结构与算法
来源：http://qzr.zdbjq.cn

================================================================================
来源：http://fym.chenlongwang.top

[N01] 二分查找（有序数组）
来源：http://qtg.hywenlv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uwf.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vuf.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ayc.cdnleiting.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qrv.52xcode.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zlm.0kj1m.cn

Go:   sort.SearchInts(arr, x)
来源：http://zdc.hfpthk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tuw.jqgfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://rwr.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://eoz.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://xmg.pycfn.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wvu.jqgufenzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nzz.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hbv.chenjidiqi.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xvc.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://feu.sysykeji.top

Ruby: arr.sort
来源：http://mko.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://btl.yj202588.top

[N03] 快速排序（分治示例）
来源：http://ske.uphjek.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fhd.uphjek.com

PHP:  // 递归实现，或用 usort
来源：http://rvo.cucudq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zka.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xcp.yj20258888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zgt.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kkj.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ifc.sxryk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dyw.shuidangran.top

[N04] 斐波那契数列
来源：http://ohi.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ulu.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cmj.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iko.52xcode.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bei.jianghu66.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kfz.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nwy.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ajt.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nqf.aizwys.cn


<!-- 参考信息 -->