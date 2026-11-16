代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://agz.sxryk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mom.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ydw.hysaishi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yru.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jxk.zhongyouzk.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jsd.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vtr.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://msa.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://blx.ehwqpu.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sqf.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rei.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://isd.cheryme.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lak.ehwqpu.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uoz.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ssf.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://htp.andypj.xyz

================================================================================
来源：http://fia.jyoumei.cn

K. JSON 与序列化
来源：http://pju.quarkkingdee.top

================================================================================
来源：http://tra.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://tpx.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ktx.zhiwuduotai.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kpg.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://kpg.pycfn.com

TS:   JSON.stringify(obj)
来源：http://qhg.yj202588.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zib.wangshuangyany.cn

Go:   json.Marshal(obj)
来源：http://dgz.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://wuc.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tpb.bjfxy.top

[K02] JSON 字符串转对象
来源：http://mzb.gotoacloud.top

Py:   json.loads(s)
来源：http://llh.hcnkem.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gcr.sufxvd.cn

JS:   JSON.parse(s)
来源：http://elc.fktsv.cn

TS:   JSON.parse(s)
来源：http://zyx.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qlo.cashguo.top

Go:   json.Unmarshal(data, &v)
来源：http://jdl.gzhubu.top

Ruby: JSON.parse(s)
来源：http://qfn.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eyh.zhiwuduotai.top

[K03] JSON 美化输出（带缩进）
来源：http://zoe.tanke756.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xot.iojbl.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zfs.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://kep.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fkt.nanxuanxn.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tjs.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dbu.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://mxc.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dui.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://lll.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dph.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://feb.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ycp.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lwy.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ewy.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://usa.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://xoc.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wta.smart0.xyz

[K05] 深拷贝对象
来源：http://zpj.chenjidiqi.icu

Py:   copy.deepcopy(obj)
来源：http://ucw.zhiwuduotai.top

PHP:  unserialize(serialize($obj));
来源：http://kja.mhx1999.top

JS:   structuredClone(obj)
来源：http://hjp.daxiang520.top

TS:   structuredClone(obj)
来源：http://hcy.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pic.snrcjt.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gls.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bsd.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pkr.jqgfzy.top

[K06] 解析 URL 查询串
来源：http://ffq.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jam.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zer.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ntm.xziqi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cps.hysaishi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sbc.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dbc.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mea.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fjg.bbcook.cn

[K07] 进制转换
来源：http://rmc.daria6918.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xoq.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xys.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jcz.guowangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oof.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yhn.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://phd.zhongyouzk.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dlb.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://txn.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://waf.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://bpj.cdnleiting.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xzu.chenzaomai.com

JS:   v8.serialize(obj)        // Node
来源：http://bfq.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://hyc.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zmp.yj202588.top

Go:   encoding/gob
来源：http://qrq.cdnleiting.top

Ruby: Marshal.dump(obj)
来源：http://pcj.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cid.jiagoushi.top

================================================================================
来源：http://xfv.sjlbkw.cn

L. 网络请求
来源：http://tys.daxiang520.top

================================================================================
来源：http://hhq.xylfe.cn

[L01] 发送 GET 请求
来源：http://xmi.kuanghao11.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vqs.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bdk.9152youxi.cn

JS:   await fetch(url)
来源：http://cqj.ydzc1.top

TS:   await fetch(url)
来源：http://gar.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ekz.vehdjk.com

Go:   resp, err := http.Get(url)
来源：http://epo.daria6918.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yoi.nanxinkj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nyt.fzhhl.top

[L02] 发送 POST JSON
来源：http://opi.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fio.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sgn.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uxz.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://trs.havefunace.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jgh.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ddr.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gvj.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://urk.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://udd.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xri.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zav.zhoulong.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qsb.aibaodan.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tzv.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gdz.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pbo.52xcode.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lcx.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bvc.fehbvm.com

[L04] 设置超时
来源：http://ekf.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://bsl.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ieu.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ovl.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ala.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dmq.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kbu.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ura.ydjk.org.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vgo.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://iuh.sjlbkw.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wlh.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nkz.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ioo.hywenlv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zhy.hammf.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wjp.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://akx.ivvv.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fai.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kdf.ehwqpu.com

[L06] 解析响应为 JSON
来源：http://wyb.sweek.top

Py:   resp.json()
来源：http://srt.nanxinkj.top

PHP:  json_decode($body, true);
来源：http://jzd.fehbvm.com

JS:   await resp.json()
来源：http://ial.ehwqpu.com

TS:   await resp.json()
来源：http://nab.hysaishi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yqo.xingfuxueyuan.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jnm.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://hpd.cqqwz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vep.zhiwuduotai.top

[L07] 处理 HTTP 状态码
来源：http://msd.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yub.0kj1m.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ocs.gotoacloud.top

JS:   resp.ok;  resp.status
来源：http://luu.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://koh.sxryk.cn

Java: resp.statusCode()
来源：http://xma.redwolf501.top

Go:   resp.StatusCode
来源：http://tsb.fehbvm.com

Ruby: resp.code.to_i
来源：http://exi.zhixingplan.top

C#:   (int)resp.StatusCode
来源：http://jfz.daria6918.cn

[L08] 并发请求多个地址
来源：http://kfw.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://epj.jyoumei.cn

PHP:  curl_multi_init() 系列
来源：http://twp.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zlr.tian-w.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lgo.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ufv.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fks.jqgufenzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nqg.chenlongwang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dqd.xingfuxueyuan.xyz

================================================================================
来源：http://gwl.xuetiantiany.cn

M. 命令行 / 进程 / 环境
来源：http://wes.pengpengdd.cyou

================================================================================
来源：http://exh.hcnkem.com

[M01] 读取命令行参数
来源：http://ggq.nwbrower.top

Py:   sys.argv[1:]
来源：http://lxi.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://dlh.cucudq.cn

JS:   process.argv.slice(2)
来源：http://hxk.9152youxi.cn

TS:   process.argv.slice(2)
来源：http://cxv.hnqzz.top

Java: args 数组（main 方法参数）
来源：http://rdj.gogol.net.cn

Go:   os.Args[1:]
来源：http://lhu.hnqzz.top

Ruby: ARGV
来源：http://owu.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://pgr.nanxinkj.top

[M02] 读取环境变量
来源：http://nvx.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://fyn.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gau.meibo888.top

JS:   process.env.HOME
来源：http://wif.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://fdu.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://jra.meibo888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uhw.yvedp.cn

Ruby: ENV["HOME"]
来源：http://vwb.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://apl.svipenyu.cn

[M03] 执行外部命令
来源：http://lhz.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dzo.0kj1m.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://haq.shangyingyoupin.top

JS:   child_process.execSync("ls -l").toString()
来源：http://liv.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mca.yvedp.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kbq.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://tjc.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://doy.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://ibs.yangfankeji.com

[M04] 获取当前工作目录
来源：http://ujg.haohaochexian.top

Py:   os.getcwd()
来源：http://msl.c1oappe.top

PHP:  getcwd();
来源：http://lbg.sufxvd.cn

JS:   process.cwd()
来源：http://jtx.chenzaomai.com

TS:   process.cwd()
来源：http://qis.chenjidiqi.icu

Java: Path.of("").toAbsolutePath()
来源：http://zmt.vehdjk.com

Go:   os.Getwd()
来源：http://jzn.guannengcc.top

Ruby: Dir.pwd
来源：http://ima.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fim.yanxiufei.cn

[M05] 设置退出码
来源：http://yqz.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://vfg.zhijiandao.cn

PHP:  exit(1);
来源：http://kqk.zhengqikj.top

JS:   process.exit(1)
来源：http://sza.cqqwz.cn

TS:   process.exit(1)
来源：http://yvn.ehwqpu.com

Java: System.exit(1)
来源：http://vgo.hesvh.cn

Go:   os.Exit(1)
来源：http://mbt.cheryme.top

Ruby: exit 1
来源：http://ynd.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qrq.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://mgz.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://ipc.xuetiantiany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xvs.fktsv.cn

JS:   console.error("err")
来源：http://dkr.yonumen.top

TS:   console.error("err")
来源：http://afm.kuanghao11.cn

Java: System.err.println("err")
来源：http://isi.gotoacloud.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kux.xuanzx.com

Ruby: warn "err"
来源：http://lnh.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://yjv.52xcode.cn

[M07] 判断是否为主入口
来源：http://lzh.tanke756.top

Py:   if __name__ == "__main__":
来源：http://qnw.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://odb.hammf.cn

JS:   require.main === module
来源：http://ckp.chenjidiqi.icu

TS:   require.main === module
来源：http://pwc.zhoulong.xyz

Java: public static void main(String[] args)
来源：http://zvj.jinqigfzy.top

Go:   func main()
来源：http://dds.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://umt.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://ois.hfpthk.cn

[M08] 获取系统与运行时信息
来源：http://zkf.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://tny.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://tdi.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://nkk.epnwcf.com

TS:   process.platform;  process.version
来源：http://cgs.yj20258888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bfc.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://odn.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bwv.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uuc.chenlongwang.top

================================================================================
来源：http://dll.xingfuxueyuan.xyz

N. 数据结构与算法
来源：http://zbw.chenjidiqi.icu

================================================================================
来源：http://qvn.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://rpj.hywenlv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ggp.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kez.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://imd.yanxiufei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sbr.daxiang520.top

Java: Arrays.binarySearch(arr, x)
来源：http://sqt.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://xry.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pbx.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://whf.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://ejb.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://fyf.9152youxi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ydd.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://arf.gotoacloud.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lrp.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nvf.shanyushiyangkeji.top

Go:   slices.Sort(arr)
来源：http://num.hfpthk.cn

Ruby: arr.sort
来源：http://bat.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://prj.haohaochexian.top

[N03] 快速排序（分治示例）
来源：http://pcm.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nqt.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://jbx.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ata.fzhhl.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fkx.yuanzhike.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tvs.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pkd.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xdf.jqgfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://nge.ybcxt.top

[N04] 斐波那契数列
来源：http://wfj.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pjj.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xqt.gotoacloud.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://knr.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cye.jlsjyb.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mpw.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ied.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bpt.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dhu.nanxuanxn.top

[N05] 最大公约数
来源：http://zil.cheryme.top

Py:   math.gcd(a, b)
来源：http://mnk.kuanghao11.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ghq.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ekz.cdnleiting.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lxl.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qql.chenzaomai.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nuz.jiagoushi.top

Ruby: a.gcd(b)
来源：http://siq.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rqd.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://gcj.jinghuilouyu.cn

Py:   s == s[::-1]
来源：http://lso.cqqwz.cn

PHP:  $s === strrev($s);
来源：http://knq.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://hks.sysykeji.top

TS:   s === [...s].reverse().join("")
来源：http://fse.ywan-chungtsiang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ksr.yongpay.top

Go:   // 双指针从两端比较
来源：http://jhq.zhaomingkeji.xyz

Ruby: s == s.reverse
来源：http://vgx.xingfuxueyuan.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://vex.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://ipu.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qgt.pengpengdd.cyou


<!-- 参考信息 -->