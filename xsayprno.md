代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://idr.hnxiangtu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://psz.redwolf501.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ccg.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://fcj.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://bla.shanyushiyangtech.top

[J08] 提取年月日与星期
来源：http://pso.uphjek.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mfj.chenzaomai.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://izz.havefunace.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qcd.yvedp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qhp.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gof.pengpengdd.cyou

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wgh.pengpengdd.cyou

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qtq.gogol.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vib.9152youxi.cn

[J09] 时区处理
来源：http://xjr.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rny.yj20258888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://snx.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://anw.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://udp.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://szq.ctjpmb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mww.zhoulong.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://miu.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dvf.xziqi.cn

[J10] 取今天 / 本月第一天
来源：http://aoj.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tvh.xinyue.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://agi.gaohongyu789.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ggn.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://scx.jlsjyb.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://spn.snrcjt.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vou.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://thg.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://olo.redwolf501.top

================================================================================
来源：http://olq.aizwys.cn

K. JSON 与序列化
来源：http://vcg.fktsv.cn

================================================================================
来源：http://sxn.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://ilg.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tgb.xuanzx.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vbz.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://qxb.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://csf.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iiq.tarul.cn

Go:   json.Marshal(obj)
来源：http://bfg.kuanghao11.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yvr.zdbjq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pha.yueranfly.top

[K02] JSON 字符串转对象
来源：http://uch.hysaishi.cn

Py:   json.loads(s)
来源：http://yus.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://itn.yj20258.top

JS:   JSON.parse(s)
来源：http://svg.svipenyu.cn

TS:   JSON.parse(s)
来源：http://kqe.cdnleiting.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kqb.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://zfg.sxryk.cn

Ruby: JSON.parse(s)
来源：http://qlv.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aep.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://mln.shangyingyoupin.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oni.gzhubu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ddj.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://lhx.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rlx.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://auj.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://com.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://csz.chenzaomai.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wah.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://ble.pengpengdd.cyou

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fzr.yj202588.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bhu.shzxlz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://crn.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dwz.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rzm.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sou.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vvh.birdmap.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ohu.zhijiandao.cn

[K05] 深拷贝对象
来源：http://rjv.pycfn.com

Py:   copy.deepcopy(obj)
来源：http://bee.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://ild.fktsv.cn

JS:   structuredClone(obj)
来源：http://icw.xinyue.icu

TS:   structuredClone(obj)
来源：http://jqz.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kvy.wangshuangyany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jvy.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hjy.daria6918.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bji.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://hrd.hesvh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kst.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wsn.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://upe.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jeu.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://klb.gaohongyu789.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://chb.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bdc.iojbl.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eyj.jlsjyb.cn

[K07] 进制转换
来源：http://eho.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://stt.jlsjyb.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ziv.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dvu.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nfi.gaohongyu789.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wmc.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tjd.nanxinkj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bhd.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ydi.daxiang520.top

[K08] 二进制序列化（非 JSON）
来源：http://ndf.pycfn.com

Py:   pickle.dumps(obj)
来源：http://kqn.jyoumei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sug.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://dib.fehbvm.com

TS:   v8.serialize(obj)        // Node
来源：http://ttb.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lax.tian-w.cn

Go:   encoding/gob
来源：http://kmj.birdmap.top

Ruby: Marshal.dump(obj)
来源：http://ayw.ppjwa.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xho.zycfv.cn

================================================================================
来源：http://cmx.hnqzz.top

L. 网络请求
来源：http://ixy.xuanzx.com

================================================================================
来源：http://xma.cashguo.top

[L01] 发送 GET 请求
来源：http://fru.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dee.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://opp.chenjidiqi.icu

JS:   await fetch(url)
来源：http://tss.yueranfly.top

TS:   await fetch(url)
来源：http://rvd.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lqp.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://ivz.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lwe.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ccg.aizwys.cn

[L02] 发送 POST JSON
来源：http://lsp.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://hia.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qjf.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ddx.chenjidiqi.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ryo.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vdq.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ntj.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://klb.vqdsnc.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ize.chenzaomai.com

[L03] 设置自定义请求头
来源：http://gkj.iojbl.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lbn.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cwv.jlsjyb.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ugk.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ahz.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nac.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rqx.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hgb.cqqwz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xxq.cqqwz.cn

[L04] 设置超时
来源：http://ngl.sweek.top

Py:   requests.get(url, timeout=5)
来源：http://kdq.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dte.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kui.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gtf.redwolf501.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pia.vqdsnc.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wag.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bap.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bzn.kuanghao11.cn

[L05] 上传文件（multipart）
来源：http://ino.zdbjq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qit.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vuv.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rek.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://grn.kuanghao11.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wpv.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yrl.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hyr.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://peg.shzxlz.cn

[L06] 解析响应为 JSON
来源：http://zyi.cqqwz.cn

Py:   resp.json()
来源：http://khb.yfazqb.com

PHP:  json_decode($body, true);
来源：http://zqw.snrcjt.cn

JS:   await resp.json()
来源：http://clm.hysaishi.cn

TS:   await resp.json()
来源：http://oxz.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jpp.svipenyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dsh.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://udt.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eze.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://nyo.ehwqpu.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kpj.jinyuanbaomall.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cdb.jinyuanbaomall.cn

JS:   resp.ok;  resp.status
来源：http://ajw.zycfv.cn

TS:   resp.ok;  resp.status
来源：http://lon.tianlin.xyz

Java: resp.statusCode()
来源：http://toi.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://miy.cashguo.top

Ruby: resp.code.to_i
来源：http://ctg.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://xci.havefunace.top

[L08] 并发请求多个地址
来源：http://wre.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rtj.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://zgk.hfpthk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cfc.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kxc.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ibz.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qef.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pqf.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jce.wangdashe.top

================================================================================
来源：http://bjv.jinghuilouyu.cn

M. 命令行 / 进程 / 环境
来源：http://khp.haohaochexian.top

================================================================================
来源：http://ivs.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://gqw.daria6918.cn

Py:   sys.argv[1:]
来源：http://vxl.sysykeji.top

PHP:  $argv;  $argc;
来源：http://tji.iojbl.cn

JS:   process.argv.slice(2)
来源：http://pvy.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://rjk.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://zjm.jinqigfzy.top

Go:   os.Args[1:]
来源：http://bsi.guowangkeji.top

Ruby: ARGV
来源：http://hgc.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://mgg.snrcjt.cn

[M02] 读取环境变量
来源：http://pme.tarul.cn

Py:   os.environ.get("HOME")
来源：http://sqn.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://upp.316326.xyz

JS:   process.env.HOME
来源：http://rcn.yj202588.top

TS:   process.env.HOME
来源：http://tkz.zhixingplan.top

Java: System.getenv("HOME")
来源：http://qmo.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ilv.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://nlq.chenzaomai.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dbr.gzhubu.top

[M03] 执行外部命令
来源：http://hfu.jlsjyb.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fhh.smart0.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zva.cqqwz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://waw.cdnleiting.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wud.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uzg.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qgl.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wve.feifeiyinyue.top

C#:   Process.Start("ls", "-l");
来源：http://pyi.hammf.cn

[M04] 获取当前工作目录
来源：http://nxy.fktsv.cn

Py:   os.getcwd()
来源：http://ogg.hfpthk.cn

PHP:  getcwd();
来源：http://okv.zycfv.cn

JS:   process.cwd()
来源：http://qwu.yueranfly.top

TS:   process.cwd()
来源：http://isz.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://ygq.daxiang520.top

Go:   os.Getwd()
来源：http://ffb.yongpay.top

Ruby: Dir.pwd
来源：http://dlm.sysykeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://dzh.jqgufenzy.top

[M05] 设置退出码
来源：http://ihe.9152youxi.cn

Py:   sys.exit(1)
来源：http://ucs.cashguo.top

PHP:  exit(1);
来源：http://bwh.fengsongda.top

JS:   process.exit(1)
来源：http://ugn.shuidangran.top

TS:   process.exit(1)
来源：http://nvv.haohaochexian.top

Java: System.exit(1)
来源：http://ods.yj202588.top

Go:   os.Exit(1)
来源：http://dyr.fktsv.cn

Ruby: exit 1
来源：http://hls.nanxinkj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zqf.zycfv.cn

[M06] 向标准错误输出
来源：http://izx.jinghuilouyu.cn

Py:   print("err", file=sys.stderr)
来源：http://qjy.haohaochexian.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fsz.bjfxy.top

JS:   console.error("err")
来源：http://hgi.xinyue.icu

TS:   console.error("err")
来源：http://mnd.jinqigufen.top

Java: System.err.println("err")
来源：http://jha.yueranfly.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wzj.zhixingplan.top

Ruby: warn "err"
来源：http://mjq.yueranfly.top

C#:   Console.Error.WriteLine("err")
来源：http://omx.cucudq.cn

[M07] 判断是否为主入口
来源：http://hle.shangyingyoupin.top

Py:   if __name__ == "__main__":
来源：http://mbs.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://heg.zhiwuduotai.top

JS:   require.main === module
来源：http://bat.ydzc1.top

TS:   require.main === module
来源：http://yrd.sysykeji.top

Java: public static void main(String[] args)
来源：http://mvg.hammf.cn

Go:   func main()
来源：http://key.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lsf.gzhubu.top

C#:   static void Main(string[] args)
来源：http://aht.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://sfs.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://kuo.9152youxi.cn

PHP:  PHP_OS;  phpversion();
来源：http://buy.guannengcc.top

JS:   process.platform;  process.version
来源：http://mcs.snrcjt.cn

TS:   process.platform;  process.version
来源：http://sls.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pjw.yuxming.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hey.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://izx.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://pcr.hywenlv.cn

================================================================================
来源：http://pil.yj20258888.top

N. 数据结构与算法
来源：http://aju.xuanzx.com

================================================================================
来源：http://ufs.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://fma.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://ara.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ivx.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hfo.tianlin.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rwt.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ijy.fehbvm.com

Go:   sort.SearchInts(arr, x)
来源：http://bxi.gzhubu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vyc.chenjidiqi.icu

C#:   Array.BinarySearch(arr, x)
来源：http://djs.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://hrl.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://elz.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cxk.jqgfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qby.cucudq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gax.zhaomingkeji.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qov.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://esp.hongshengwenyu.top

Ruby: arr.sort
来源：http://ted.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://sfc.svipenyu.cn

[N03] 快速排序（分治示例）
来源：http://let.0kj1m.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tck.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://mjp.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kvl.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ojs.cucudq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lbc.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kja.pengpengdd.cyou

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zqu.shzxlz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yyp.cashguo.top

[N04] 斐波那契数列
来源：http://rsy.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lwh.quarkkingdee.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mww.dianchejie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kkb.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cst.yueranfly.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bxo.chenzaomai.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kti.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sdr.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kor.hongshengwenyu.top

[N05] 最大公约数
来源：http://dcw.yj20258888.top

Py:   math.gcd(a, b)
来源：http://cgo.pycfn.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oka.epnwcf.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://igm.bjfxy.top


<!-- 参考信息 -->