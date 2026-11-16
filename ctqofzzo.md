代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ape.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ukr.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kgp.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://kdx.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://vok.epnwcf.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ubp.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dij.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://btr.hysaishi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wzx.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wss.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qyo.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://edf.yonumen.top

================================================================================
来源：http://lat.vqdsnc.cn

K. JSON 与序列化
来源：http://nfs.0kj1m.cn

================================================================================
来源：http://syz.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://lnn.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lel.tianlin.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nqu.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://fzi.tian-w.cn

TS:   JSON.stringify(obj)
来源：http://jkq.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ilr.yongpay.top

Go:   json.Marshal(obj)
来源：http://sgl.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vfo.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ase.smart0.xyz

[K02] JSON 字符串转对象
来源：http://ugc.zycfv.cn

Py:   json.loads(s)
来源：http://pou.snrcjt.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zzc.vehdjk.com

JS:   JSON.parse(s)
来源：http://gpt.haohaochexian.top

TS:   JSON.parse(s)
来源：http://yao.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cgq.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://xqr.cheryme.top

Ruby: JSON.parse(s)
来源：http://evy.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fra.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://bwt.smart0.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zbm.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://idt.52xcode.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hop.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tpj.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mfb.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bub.daxiang520.top

Ruby: JSON.pretty_generate(obj)
来源：http://idl.aibaodan.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tvm.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://vrg.hongshengwenyu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lht.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uxi.xuetiantiany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wfj.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kgn.yj20258.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rkp.fzhhl.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ets.hywenlv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zam.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uly.vehdjk.com

[K05] 深拷贝对象
来源：http://kgd.smart0.xyz

Py:   copy.deepcopy(obj)
来源：http://vhj.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://brm.chenjidiqi.icu

JS:   structuredClone(obj)
来源：http://ljn.ydzc1.top

TS:   structuredClone(obj)
来源：http://axl.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lkl.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://izs.yongpay.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mnx.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://osa.ivvv.top

[K06] 解析 URL 查询串
来源：http://dhc.chenlongwang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ogd.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gqb.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://btk.cdnleiting.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lmi.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dar.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://utz.pengpengdd.cyou

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://omn.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nwd.hnxiangtu.top

[K07] 进制转换
来源：http://tob.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dzk.gogol.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dms.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tsw.zycfv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dga.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wuo.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ujt.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mqj.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yfo.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://obe.ydjk.org.cn

Py:   pickle.dumps(obj)
来源：http://asl.sufxvd.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cor.jiagoushi.top

JS:   v8.serialize(obj)        // Node
来源：http://smr.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://brh.yj202588.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qnh.aibaodan.cn

Go:   encoding/gob
来源：http://fbc.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://uos.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nvb.jlsjyb.cn

================================================================================
来源：http://sbc.chenzaomai.com

L. 网络请求
来源：http://ijb.zycfv.cn

================================================================================
来源：http://lxe.mhx1999.top

[L01] 发送 GET 请求
来源：http://bqt.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wji.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iaf.zdqjudy.top

JS:   await fetch(url)
来源：http://llk.hywenlv.cn

TS:   await fetch(url)
来源：http://ssp.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gwd.shzxlz.cn

Go:   resp, err := http.Get(url)
来源：http://qlj.hnxiangtu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tnl.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://see.yangfankeji.com

[L02] 发送 POST JSON
来源：http://aao.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qfq.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jyf.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kvh.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tbi.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qvc.gaohongyu789.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hpf.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://abm.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lhy.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://tzw.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dma.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ulz.hcnkem.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bag.nanxinkj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xbf.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yix.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kth.52xcode.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ckv.ybcxt.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wop.yvedp.cn

[L04] 设置超时
来源：http://rsv.haohaochexian.top

Py:   requests.get(url, timeout=5)
来源：http://mcl.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zwn.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tdo.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gel.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ipo.shanyushiyangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dgo.zdbjq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uyz.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bxh.cheryme.top

[L05] 上传文件（multipart）
来源：http://wid.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nbb.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zsc.hcnkem.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://odf.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yfs.sxryk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fpi.shzxlz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rei.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ken.jiagoushi.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://axg.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://duw.andypj.xyz

Py:   resp.json()
来源：http://iln.daria6918.cn

PHP:  json_decode($body, true);
来源：http://doq.yj202588.top

JS:   await resp.json()
来源：http://olv.zdbjq.cn

TS:   await resp.json()
来源：http://fve.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nvs.zhoulong.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://opf.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://fab.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://htl.chenzaomai.com

[L07] 处理 HTTP 状态码
来源：http://qii.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jeq.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kzy.yj202588.top

JS:   resp.ok;  resp.status
来源：http://gjh.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://brp.cheryme.top

Java: resp.statusCode()
来源：http://oek.daria6918.cn

Go:   resp.StatusCode
来源：http://dek.fengsongda.top

Ruby: resp.code.to_i
来源：http://btf.sjlbkw.cn

C#:   (int)resp.StatusCode
来源：http://noj.tianlin.xyz

[L08] 并发请求多个地址
来源：http://rup.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gah.fzhhl.top

PHP:  curl_multi_init() 系列
来源：http://pof.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gby.hywenlv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zif.epnwcf.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ibk.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ytd.zhijiandao.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gkp.zdqjudy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mxv.birdmap.top

================================================================================
来源：http://ggc.hongshengwenyu.top

M. 命令行 / 进程 / 环境
来源：http://fzm.ehwqpu.com

================================================================================
来源：http://jub.zdqjudy.top

[M01] 读取命令行参数
来源：http://lrj.xziqi.cn

Py:   sys.argv[1:]
来源：http://tyx.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://pnk.bbcook.cn

JS:   process.argv.slice(2)
来源：http://noz.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://gzk.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://azm.wangdashe.top

Go:   os.Args[1:]
来源：http://qdi.vehdjk.com

Ruby: ARGV
来源：http://upm.cheryme.top

C#:   args 数组（Main 方法参数）
来源：http://flb.zhongyouzk.top

[M02] 读取环境变量
来源：http://uvw.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://emp.jianghu66.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zvv.wangdashe.top

JS:   process.env.HOME
来源：http://ztd.jiagoushi.top

TS:   process.env.HOME
来源：http://rrc.yfazqb.com

Java: System.getenv("HOME")
来源：http://eye.fengsongda.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nnd.yfazqb.com

Ruby: ENV["HOME"]
来源：http://wpm.chenzaomai.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gpk.dianchejie.cn

[M03] 执行外部命令
来源：http://srx.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xjx.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yvs.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wlm.yuanzhike.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ybe.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lnz.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uty.chenjidiqi.icu

Ruby: system("ls -l");  `ls -l`
来源：http://rwq.haohaochexian.top

C#:   Process.Start("ls", "-l");
来源：http://zex.gotoacloud.top

[M04] 获取当前工作目录
来源：http://ovh.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://gcq.shanyushiyangtech.top

PHP:  getcwd();
来源：http://xez.ybcxt.top

JS:   process.cwd()
来源：http://toq.chenjidiqi.icu

TS:   process.cwd()
来源：http://sws.yvedp.cn

Java: Path.of("").toAbsolutePath()
来源：http://ppw.yuanzhike.top

Go:   os.Getwd()
来源：http://xfj.guannengcc.top

Ruby: Dir.pwd
来源：http://cir.316326.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://obi.fehbvm.com

[M05] 设置退出码
来源：http://pfh.iojbl.cn

Py:   sys.exit(1)
来源：http://rib.uphjek.com

PHP:  exit(1);
来源：http://mfq.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://cst.zhoulong.xyz

TS:   process.exit(1)
来源：http://pfc.xuetiantiany.cn

Java: System.exit(1)
来源：http://atc.yuxming.cn

Go:   os.Exit(1)
来源：http://vhh.cheryme.top

Ruby: exit 1
来源：http://xkk.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ljz.zdqjudy.top

[M06] 向标准错误输出
来源：http://dze.pengpengdd.cyou

Py:   print("err", file=sys.stderr)
来源：http://zqo.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ssc.zhiwuduotai.top

JS:   console.error("err")
来源：http://jiv.ybcxt.top

TS:   console.error("err")
来源：http://xzw.shzxlz.cn

Java: System.err.println("err")
来源：http://rnk.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xbr.ivvv.top

Ruby: warn "err"
来源：http://ixc.gotoacloud.top

C#:   Console.Error.WriteLine("err")
来源：http://obb.cheryme.top

[M07] 判断是否为主入口
来源：http://xfv.fzhhl.top

Py:   if __name__ == "__main__":
来源：http://vil.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://miw.hywenlv.cn

JS:   require.main === module
来源：http://whu.hongshengwenyu.top

TS:   require.main === module
来源：http://vnb.yongpay.top

Java: public static void main(String[] args)
来源：http://tnc.zycfv.cn

Go:   func main()
来源：http://mlg.quarkkingdee.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nqw.cheryme.top

C#:   static void Main(string[] args)
来源：http://xrw.xylfe.cn

[M08] 获取系统与运行时信息
来源：http://xkc.hcnkem.com

Py:   platform.system();  platform.python_version()
来源：http://scq.yuanzhike.top

PHP:  PHP_OS;  phpversion();
来源：http://wbn.tianlin.xyz

JS:   process.platform;  process.version
来源：http://ius.yfazqb.com

TS:   process.platform;  process.version
来源：http://cnh.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gsa.xuanzx.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://riw.snrcjt.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qqo.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://alx.jlsjyb.cn

================================================================================
来源：http://dov.yj20258.top

N. 数据结构与算法
来源：http://rfq.sysykeji.top

================================================================================
来源：http://qpk.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://kpm.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://cdo.jlsjyb.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tzt.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oul.shzxlz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vfi.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://ftm.yanxiufei.cn

Go:   sort.SearchInts(arr, x)
来源：http://exk.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cgv.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rpy.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://ebo.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://xnv.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ajn.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ivh.yangfankeji.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://rgc.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kah.fengsongda.top

Go:   slices.Sort(arr)
来源：http://vaa.316326.xyz

Ruby: arr.sort
来源：http://azv.snrcjt.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ddt.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://jjb.ydjk.org.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eej.fehbvm.com

PHP:  // 递归实现，或用 usort
来源：http://dfu.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jjd.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kxs.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xzx.zhixingplan.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tia.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pzz.fanxiaobao.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://weg.snrcjt.cn

[N04] 斐波那契数列
来源：http://yok.ctjpmb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ipi.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ksc.zycfv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sew.yvedp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://txx.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lnt.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yqa.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nsk.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pbc.hongshengwenyu.top

[N05] 最大公约数
来源：http://vbf.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://tzk.zhengqikj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://peo.hfpthk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qbz.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ryw.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ovh.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vxd.haohaochexian.top

Ruby: a.gcd(b)
来源：http://qbp.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cif.9152youxi.cn

[N06] 判断回文字符串
来源：http://bdt.jlsjyb.cn

Py:   s == s[::-1]
来源：http://cxr.52xcode.cn

PHP:  $s === strrev($s);
来源：http://zud.shangyingyoupin.top

JS:   s === [...s].reverse().join("")
来源：http://bqq.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://ewc.xinyue.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blg.iojbl.cn

Go:   // 双指针从两端比较
来源：http://ewq.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://vbu.jinghuilouyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ezg.sufxvd.cn

[N07] 两数之和（返回下标）
来源：http://wtj.yueranfly.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sxx.yueranfly.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fip.nanxinkj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://reu.hongshengwenyu.top

TS:   // 手写 Map<string, number>
来源：http://nuq.svipenyu.cn

Java: // 手写 HashMap
来源：http://mtf.pycfn.com


<!-- 参考信息 -->