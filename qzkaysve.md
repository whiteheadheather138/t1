代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iok.birdmap.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zgk.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oip.hnqzz.top

[J10] 取今天 / 本月第一天
来源：http://zqa.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qjy.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://way.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wul.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hxf.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ibq.fanxiaobao.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iyn.chenjidiqi.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pnv.hysaishi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ipf.gaohongyu789.top

================================================================================
来源：http://gjk.guannengcc.top

K. JSON 与序列化
来源：http://erk.cucudq.cn

================================================================================
来源：http://nll.daria6918.cn

[K01] 对象转 JSON 字符串
来源：http://rwf.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oso.meibo888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wsb.yfazqb.com

JS:   JSON.stringify(obj)
来源：http://ibz.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://cen.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rzy.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://uwz.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ufa.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qhs.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://zlm.xingfuxueyuan.xyz

Py:   json.loads(s)
来源：http://wnh.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://upr.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://cel.fehbvm.com

TS:   JSON.parse(s)
来源：http://fjx.yfazqb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hmx.hcnkem.com

Go:   json.Unmarshal(data, &v)
来源：http://mqs.meibo888.top

Ruby: JSON.parse(s)
来源：http://mfz.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zph.haohaochexian.top

[K03] JSON 美化输出（带缩进）
来源：http://rfd.kuanghao11.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bay.tanke756.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wqv.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ddg.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rre.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://spw.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cpq.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://kng.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qme.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://jlw.hongshengwenyu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wiu.pengpengdd.cyou

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kev.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iag.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kto.smart0.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ava.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yvu.hnqzz.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ufx.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://czs.vehdjk.com

[K05] 深拷贝对象
来源：http://hir.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://btn.xylfe.cn

PHP:  unserialize(serialize($obj));
来源：http://vrj.shzxlz.cn

JS:   structuredClone(obj)
来源：http://gmf.chenzaomai.com

TS:   structuredClone(obj)
来源：http://kiu.pengpengdd.cyou

Java: // 手写拷贝构造，或序列化往返
来源：http://iva.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://udn.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://myz.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qio.jinqigfzy.top

[K06] 解析 URL 查询串
来源：http://kdc.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zrw.ivvv.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mbp.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xpl.zhijiandao.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tkk.gzhubu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pnh.yuxming.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://waa.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eod.kuanghao11.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yrs.ehwqpu.com

[K07] 进制转换
来源：http://ocq.snrcjt.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gff.fktsv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zfb.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sma.hywenlv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yoi.hesvh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://diy.shuidangran.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bue.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yjm.havefunace.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lxu.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://rbo.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://bzj.jqgfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pdz.gzhubu.top

JS:   v8.serialize(obj)        // Node
来源：http://hmj.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://nof.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ifc.yonumen.top

Go:   encoding/gob
来源：http://nuz.xylfe.cn

Ruby: Marshal.dump(obj)
来源：http://pss.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nri.shanyushiyangtech.top

================================================================================
来源：http://oej.dashuyun.cn

L. 网络请求
来源：http://pfa.ywan-chungtsiang.top

================================================================================
来源：http://nvc.wangdashe.top

[L01] 发送 GET 请求
来源：http://fch.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://omk.shanyushiyangtech.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yuj.jiagoushi.top

JS:   await fetch(url)
来源：http://cug.quarkkingdee.top

TS:   await fetch(url)
来源：http://gwl.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ntu.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://gcz.nwbrower.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jtk.cheryme.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pvp.gaohongyu789.top

[L02] 发送 POST JSON
来源：http://otd.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://epy.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gvo.pengpengdd.cyou

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ayf.chenjidiqi.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tri.ivvv.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ynn.fanxiaobao.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iow.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xox.feifeiyinyue.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://obi.smart0.xyz

[L03] 设置自定义请求头
来源：http://rws.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://epm.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nxp.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fwe.jinyuanbaomall.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fdk.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vtj.iojbl.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dhn.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vgp.316326.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rlf.uphjek.com

[L04] 设置超时
来源：http://dzj.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://ihs.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ufo.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ohm.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qhs.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yxb.tian-w.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dgh.haohaochexian.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mkl.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zem.pycfn.com

[L05] 上传文件（multipart）
来源：http://qhp.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ipo.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yqk.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cjw.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bdm.gotoacloud.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ntx.bjfxy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://klu.tianlin.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tyr.ywan-chungtsiang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ukt.uphjek.com

[L06] 解析响应为 JSON
来源：http://smq.jqgufenzy.top

Py:   resp.json()
来源：http://ycq.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://qao.nanxinkj.top

JS:   await resp.json()
来源：http://srt.jinqigfzy.top

TS:   await resp.json()
来源：http://xjb.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pdg.zhongyouzk.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tse.yueranfly.top

Ruby: JSON.parse(resp.body)
来源：http://srz.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xcu.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://dnz.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lhj.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cgg.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://cfr.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://edu.fktsv.cn

Java: resp.statusCode()
来源：http://ofx.meibo888.top

Go:   resp.StatusCode
来源：http://wki.jyoumei.cn

Ruby: resp.code.to_i
来源：http://tyh.gzhubu.top

C#:   (int)resp.StatusCode
来源：http://ncl.nanxinkj.top

[L08] 并发请求多个地址
来源：http://dfz.zhixingplan.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hye.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://yod.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qcl.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gjl.shzxlz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mlk.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ivf.dashuyun.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dix.aibaodan.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xtq.daria6918.cn

================================================================================
来源：http://yyz.wangshuangyany.cn

M. 命令行 / 进程 / 环境
来源：http://bnu.yj202588.top

================================================================================
来源：http://xaj.shuidangran.top

[M01] 读取命令行参数
来源：http://knr.bbcook.cn

Py:   sys.argv[1:]
来源：http://bpl.fzhhl.top

PHP:  $argv;  $argc;
来源：http://lvi.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://yol.redwolf501.top

TS:   process.argv.slice(2)
来源：http://eoq.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://nym.birdmap.top

Go:   os.Args[1:]
来源：http://ypl.hfpthk.cn

Ruby: ARGV
来源：http://xqy.sjlbkw.cn

C#:   args 数组（Main 方法参数）
来源：http://lsh.bbcook.cn

[M02] 读取环境变量
来源：http://bss.c1oappe.top

Py:   os.environ.get("HOME")
来源：http://ubh.mhx1999.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sac.fengsongda.top

JS:   process.env.HOME
来源：http://hss.jqgufenzy.top

TS:   process.env.HOME
来源：http://kpl.guowangkeji.top

Java: System.getenv("HOME")
来源：http://hjl.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ohc.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://ofj.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://trb.jianghu66.top

[M03] 执行外部命令
来源：http://gih.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kqh.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ssg.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tpw.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jlh.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://olj.fzhhl.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bjk.jyoumei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vgp.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://zez.cashguo.top

[M04] 获取当前工作目录
来源：http://squ.gzhubu.top

Py:   os.getcwd()
来源：http://tak.ctjpmb.com

PHP:  getcwd();
来源：http://npy.daxiang520.top

JS:   process.cwd()
来源：http://tjf.yfazqb.com

TS:   process.cwd()
来源：http://aet.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://ivg.gaohongyu789.top

Go:   os.Getwd()
来源：http://xtv.nanxinkj.top

Ruby: Dir.pwd
来源：http://hwl.daria6918.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lff.wangdashe.top

[M05] 设置退出码
来源：http://rbj.fanxiaobao.xyz

Py:   sys.exit(1)
来源：http://ehc.fehbvm.com

PHP:  exit(1);
来源：http://pjl.cashguo.top

JS:   process.exit(1)
来源：http://qhj.c1oappe.top

TS:   process.exit(1)
来源：http://zys.guannengcc.top

Java: System.exit(1)
来源：http://skt.hywenlv.cn

Go:   os.Exit(1)
来源：http://edi.yvedp.cn

Ruby: exit 1
来源：http://xwm.jinghuilouyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://grl.uphjek.com

[M06] 向标准错误输出
来源：http://sqj.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://wdm.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://trb.dashuyun.cn

JS:   console.error("err")
来源：http://dbt.yuanzhike.top

TS:   console.error("err")
来源：http://xkf.zhixingplan.top

Java: System.err.println("err")
来源：http://iqp.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zth.sxryk.cn

Ruby: warn "err"
来源：http://tox.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://xnk.xylfe.cn

[M07] 判断是否为主入口
来源：http://giu.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://kzn.shanyushiyangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ffw.hesvh.cn

JS:   require.main === module
来源：http://wti.aibaodan.cn

TS:   require.main === module
来源：http://qkt.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://jcy.yangfankeji.com

Go:   func main()
来源：http://gxa.yvedp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://feh.yj202588.top

C#:   static void Main(string[] args)
来源：http://ovs.yj202588.top

[M08] 获取系统与运行时信息
来源：http://wgf.hfpthk.cn

Py:   platform.system();  platform.python_version()
来源：http://yfr.kuanghao11.cn

PHP:  PHP_OS;  phpversion();
来源：http://ecl.iojbl.cn

JS:   process.platform;  process.version
来源：http://gve.iojbl.cn

TS:   process.platform;  process.version
来源：http://nct.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aos.zycfv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dum.xziqi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yfs.hesvh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nyl.fzhhl.top

================================================================================
来源：http://umo.52xcode.cn

N. 数据结构与算法
来源：http://hgs.bbcook.cn

================================================================================
来源：http://oyr.uphjek.com

[N01] 二分查找（有序数组）
来源：http://uzu.sjlbkw.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bos.gaohongyu789.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yjy.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rtv.sjlbkw.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cfx.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://crh.dashuyun.cn

Go:   sort.SearchInts(arr, x)
来源：http://pdo.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://vku.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://tes.redwolf501.top

[N02] 排序（工程实践用内置实现）
来源：http://fta.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://ark.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vab.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yad.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://zmp.ydzc1.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nbg.yanxiufei.cn

Go:   slices.Sort(arr)
来源：http://esd.hfpthk.cn

Ruby: arr.sort
来源：http://bjk.c1oappe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ikl.zhengqikj.top

[N03] 快速排序（分治示例）
来源：http://peo.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pgn.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://umk.xziqi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nsd.shzxlz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://elb.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aym.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wdt.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ltv.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dur.bbcook.cn

[N04] 斐波那契数列
来源：http://lva.dashuyun.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cja.ybcxt.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mod.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nyj.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yvl.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uqb.ppjwa.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tdz.fehbvm.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kuc.fzhhl.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gzr.0kj1m.cn

[N05] 最大公约数
来源：http://snq.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://hpc.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://acj.epnwcf.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xyy.hongshengwenyu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rht.xylfe.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zab.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jeo.meibo888.top

Ruby: a.gcd(b)
来源：http://cbv.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xwq.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://uph.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://pxr.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://mus.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://ccd.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://yiq.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lzy.sysykeji.top

Go:   // 双指针从两端比较
来源：http://lxe.jyoumei.cn

Ruby: s == s.reverse
来源：http://sjn.xingfuxueyuan.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://nul.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://ono.quarkkingdee.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jju.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rio.zycfv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jyu.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://evr.tianlin.xyz

Java: // 手写 HashMap
来源：http://ucg.52xcode.cn


<!-- 参考信息 -->