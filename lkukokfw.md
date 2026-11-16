代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://hjb.dianchejie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iwc.jinqigfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://drp.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://luk.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://ftm.svipenyu.cn

[J08] 提取年月日与星期
来源：http://yth.jyoumei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xcl.gaohongyu789.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://veu.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cgr.tanke756.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lnr.hywenlv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lwh.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qbb.cqqwz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rdc.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://stb.hongshengwenyu.top

[J09] 时区处理
来源：http://pma.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ldb.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://utz.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tuy.cheryme.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://suf.wangdashe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vtt.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rbu.epnwcf.com

Ruby: Time.now.getlocal("+08:00")
来源：http://fjc.jinqigufen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ega.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://rip.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://cqc.52xcode.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gjs.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cfa.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ikr.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xpp.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yzu.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mwr.iojbl.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://crf.ybcxt.top

================================================================================
来源：http://fkp.jyoumei.cn

K. JSON 与序列化
来源：http://ymh.sufxvd.cn

================================================================================
来源：http://iun.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://bmr.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kil.meibo888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cdn.zhoulong.xyz

JS:   JSON.stringify(obj)
来源：http://gmm.wangdashe.top

TS:   JSON.stringify(obj)
来源：http://tzh.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cxd.bbcook.cn

Go:   json.Marshal(obj)
来源：http://nqn.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dag.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uws.guowangkeji.top

[K02] JSON 字符串转对象
来源：http://xya.yuanzhike.top

Py:   json.loads(s)
来源：http://ygb.zhongyouzk.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://psd.daria6918.cn

JS:   JSON.parse(s)
来源：http://jsd.xuanzx.com

TS:   JSON.parse(s)
来源：http://tft.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gtw.ctjpmb.com

Go:   json.Unmarshal(data, &v)
来源：http://kmy.epnwcf.com

Ruby: JSON.parse(s)
来源：http://aqp.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dvs.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://ong.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ort.hywenlv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ijz.tarul.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ptl.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://mso.c1oappe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rhj.xuanzx.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://krk.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://bvg.mhx1999.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://utk.c1oappe.top

[K04] 读取 JSON 文件
来源：http://yrw.daxiang520.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hyj.guannengcc.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rxf.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bkc.bbcook.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yei.zhixingplan.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://txc.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nnz.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://szw.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fmd.fanxiaobao.xyz

[K05] 深拷贝对象
来源：http://fur.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://cuh.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://lou.shanyushiyangkeji.top

JS:   structuredClone(obj)
来源：http://yki.shuidangran.top

TS:   structuredClone(obj)
来源：http://rno.zhixingplan.top

Java: // 手写拷贝构造，或序列化往返
来源：http://npu.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hqq.ehwqpu.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://emx.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://etg.havefunace.top

[K06] 解析 URL 查询串
来源：http://enm.svipenyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ejy.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mav.jinqigufen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nfu.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rmz.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zuf.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bjd.ivvv.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lsn.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tib.xuetiantiany.cn

[K07] 进制转换
来源：http://ikz.fzhhl.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xbx.tarul.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ynp.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bzc.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rvu.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cml.aibaodan.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zzb.andypj.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aku.gzhubu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sof.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://zse.yj202588.top

Py:   pickle.dumps(obj)
来源：http://rlo.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://eur.epnwcf.com

JS:   v8.serialize(obj)        // Node
来源：http://hjg.jianghu66.top

TS:   v8.serialize(obj)        // Node
来源：http://gvg.xziqi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jnq.zhengqikj.top

Go:   encoding/gob
来源：http://upr.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://psq.shanyushiyangtech.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gle.guannengcc.top

================================================================================
来源：http://efx.dashuyun.cn

L. 网络请求
来源：http://epm.xziqi.cn

================================================================================
来源：http://ahj.vehdjk.com

[L01] 发送 GET 请求
来源：http://qbq.cashguo.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ddn.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kju.zhongyouzk.top

JS:   await fetch(url)
来源：http://ket.dianchejie.cn

TS:   await fetch(url)
来源：http://cpg.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://thx.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://uqf.fanxiaobao.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://xve.cqqwz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rdx.guowangkeji.top

[L02] 发送 POST JSON
来源：http://ouk.yangfankeji.com

Py:   requests.post(url, json={"a": 1})
来源：http://mor.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hoc.dashuyun.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qmy.wangshuangyany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://slu.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zsc.havefunace.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yct.fehbvm.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yoq.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jmn.jinghuilouyu.cn

[L03] 设置自定义请求头
来源：http://hih.yanxiufei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xhi.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lpb.tianlin.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pkm.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xrr.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ttw.cheryme.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dys.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eby.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ibc.pengpengdd.cyou

[L04] 设置超时
来源：http://ibe.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://soy.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nuq.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cvy.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://npc.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bjs.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tap.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wmk.bbcook.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pwd.cashguo.top

[L05] 上传文件（multipart）
来源：http://aln.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mzk.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tsz.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cze.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lxl.kuanghao11.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ohu.chenlongwang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xlk.jqgufenzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nwu.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rly.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://pdu.vehdjk.com

Py:   resp.json()
来源：http://zsw.fengsongda.top

PHP:  json_decode($body, true);
来源：http://gez.ctjpmb.com

JS:   await resp.json()
来源：http://bha.hnqzz.top

TS:   await resp.json()
来源：http://kvg.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://exl.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://peh.ywan-chungtsiang.top

Ruby: JSON.parse(resp.body)
来源：http://bpo.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yil.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://wox.tianlin.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sra.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xfs.tianlin.xyz

JS:   resp.ok;  resp.status
来源：http://kga.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://shl.yueranfly.top

Java: resp.statusCode()
来源：http://vry.sxryk.cn

Go:   resp.StatusCode
来源：http://rjo.yuanzhike.top

Ruby: resp.code.to_i
来源：http://bjr.316326.xyz

C#:   (int)resp.StatusCode
来源：http://fqz.nanxinkj.top

[L08] 并发请求多个地址
来源：http://vtr.hongshengwenyu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zsm.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://kpr.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iwl.andypj.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lhl.pengpengdd.cyou

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bjp.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lxh.cashguo.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rag.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wnl.fengsongda.top

================================================================================
来源：http://gad.hywenlv.cn

M. 命令行 / 进程 / 环境
来源：http://xfd.jianghu66.top

================================================================================
来源：http://kcy.jianghu66.top

[M01] 读取命令行参数
来源：http://qwd.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://ngs.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://pke.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://oha.yvedp.cn

TS:   process.argv.slice(2)
来源：http://mtt.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://wlc.jqgufenzy.top

Go:   os.Args[1:]
来源：http://ttu.ywan-chungtsiang.top

Ruby: ARGV
来源：http://syp.hfpthk.cn

C#:   args 数组（Main 方法参数）
来源：http://zea.shzxlz.cn

[M02] 读取环境变量
来源：http://ppg.shzxlz.cn

Py:   os.environ.get("HOME")
来源：http://rgj.tian-w.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zwt.wangdashe.top

JS:   process.env.HOME
来源：http://pov.jinqigufen.top

TS:   process.env.HOME
来源：http://mrx.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://dzr.epnwcf.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://anj.havefunace.top

Ruby: ENV["HOME"]
来源：http://uab.yj20258.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bsg.jqgfzy.top

[M03] 执行外部命令
来源：http://yai.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uym.yuxming.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fur.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://qkr.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dxy.fengsongda.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lpn.uphjek.com

Go:   exec.Command("ls", "-l").Output()
来源：http://xzg.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://boy.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://svg.fehbvm.com

[M04] 获取当前工作目录
来源：http://bfh.fktsv.cn

Py:   os.getcwd()
来源：http://bsx.hcnkem.com

PHP:  getcwd();
来源：http://mhb.jqgfzy.top

JS:   process.cwd()
来源：http://efa.cashguo.top

TS:   process.cwd()
来源：http://pmh.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://pac.xziqi.cn

Go:   os.Getwd()
来源：http://lup.snrcjt.cn

Ruby: Dir.pwd
来源：http://oms.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://lyl.chenzaomai.com

[M05] 设置退出码
来源：http://wqj.cheryme.top

Py:   sys.exit(1)
来源：http://mip.fanxiaobao.xyz

PHP:  exit(1);
来源：http://etn.tanke756.top

JS:   process.exit(1)
来源：http://kut.uphjek.com

TS:   process.exit(1)
来源：http://ucb.jinqigfzy.top

Java: System.exit(1)
来源：http://plz.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://wky.9152youxi.cn

Ruby: exit 1
来源：http://ews.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kgj.wangdashe.top

[M06] 向标准错误输出
来源：http://rzi.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://kho.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nbo.hywenlv.cn

JS:   console.error("err")
来源：http://sbh.hongshengwenyu.top

TS:   console.error("err")
来源：http://ytv.hfpthk.cn

Java: System.err.println("err")
来源：http://gdq.yonumen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://otq.hesvh.cn

Ruby: warn "err"
来源：http://gvw.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://dau.yuanzhike.top

[M07] 判断是否为主入口
来源：http://lpg.yongpay.top

Py:   if __name__ == "__main__":
来源：http://ymq.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tmu.xziqi.cn

JS:   require.main === module
来源：http://fcc.shangyingyoupin.top

TS:   require.main === module
来源：http://onr.0kj1m.cn

Java: public static void main(String[] args)
来源：http://cfr.jlsjyb.cn

Go:   func main()
来源：http://uzp.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bzs.shanyushiyangkeji.top

C#:   static void Main(string[] args)
来源：http://elh.shangyingyoupin.top

[M08] 获取系统与运行时信息
来源：http://wig.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://yaz.zhiwuduotai.top

PHP:  PHP_OS;  phpversion();
来源：http://dbm.jyoumei.cn

JS:   process.platform;  process.version
来源：http://hwp.yuxming.cn

TS:   process.platform;  process.version
来源：http://qoy.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eii.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pvp.yj202588.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aqx.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wxu.sjlbkw.cn

================================================================================
来源：http://gpl.xziqi.cn

N. 数据结构与算法
来源：http://hds.shuidangran.top

================================================================================
来源：http://lfd.hcnkem.com

[N01] 二分查找（有序数组）
来源：http://qal.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qut.gogol.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ohb.dianchejie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mxn.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hzr.gzhubu.top

Java: Arrays.binarySearch(arr, x)
来源：http://snw.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://zku.jinqigfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cgf.zhongyouzk.top

C#:   Array.BinarySearch(arr, x)
来源：http://xgz.xziqi.cn

[N02] 排序（工程实践用内置实现）
来源：http://nzj.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://nee.redwolf501.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yqa.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://hlo.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ien.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nfx.ydzc1.top

Go:   slices.Sort(arr)
来源：http://fpo.nwbrower.top

Ruby: arr.sort
来源：http://fbr.cdnleiting.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wiv.wangshuangyany.cn

[N03] 快速排序（分治示例）
来源：http://wnb.jinyuanbaomall.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qac.yonumen.top

PHP:  // 递归实现，或用 usort
来源：http://fab.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lbo.shangyingyoupin.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uho.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nvi.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bzl.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nct.yongpay.top

C#:   // 手写递归，或 Array.Sort
来源：http://ezr.gogol.net.cn

[N04] 斐波那契数列
来源：http://tgf.xziqi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hmq.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jnr.tanke756.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kkf.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uwf.zhijiandao.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ztb.hcnkem.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dpa.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yti.316326.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vrk.shanyushiyangtech.top

[N05] 最大公约数
来源：http://col.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://elo.cheryme.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jqj.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://msl.fengsongda.top


<!-- 参考信息 -->