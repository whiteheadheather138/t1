代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://pit.zdbjq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jqr.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wpc.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fdl.pycfn.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nvn.daxiang520.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://den.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cjo.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jwi.ppjwa.cn

================================================================================
来源：http://qdn.wangshuangyany.cn

K. JSON 与序列化
来源：http://ili.haohaochexian.top

================================================================================
来源：http://lww.cdnleiting.top

[K01] 对象转 JSON 字符串
来源：http://gvz.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rng.epnwcf.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xpj.xuetiantiany.cn

JS:   JSON.stringify(obj)
来源：http://wki.yongpay.top

TS:   JSON.stringify(obj)
来源：http://klr.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://glg.wangshuangyany.cn

Go:   json.Marshal(obj)
来源：http://gek.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://xyg.nwbrower.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tcp.hesvh.cn

[K02] JSON 字符串转对象
来源：http://nhl.gogol.net.cn

Py:   json.loads(s)
来源：http://gbn.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://puf.sysykeji.top

JS:   JSON.parse(s)
来源：http://qjm.guannengcc.top

TS:   JSON.parse(s)
来源：http://oso.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ray.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://vbt.ehwqpu.com

Ruby: JSON.parse(s)
来源：http://qox.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ida.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://iha.chenzaomai.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://amx.meibo888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wqt.zhijiandao.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://iff.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://kzg.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hua.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wkg.sufxvd.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kpq.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tqv.yongpay.top

[K04] 读取 JSON 文件
来源：http://zjx.sjlbkw.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bol.jqgufenzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bap.yj202588.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vyh.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fib.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rtb.zhixingplan.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yyq.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zzq.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hee.fanxiaobao.xyz

[K05] 深拷贝对象
来源：http://qlv.yvedp.cn

Py:   copy.deepcopy(obj)
来源：http://sfk.hywenlv.cn

PHP:  unserialize(serialize($obj));
来源：http://mkr.chenjidiqi.icu

JS:   structuredClone(obj)
来源：http://gvv.redwolf501.top

TS:   structuredClone(obj)
来源：http://ntt.hnxiangtu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pds.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cun.jinqigufen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mnu.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qyj.meibo888.top

[K06] 解析 URL 查询串
来源：http://ech.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cww.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uws.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zzj.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lcx.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hle.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rsb.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rfv.pengpengdd.cyou

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gbk.tianlin.xyz

[K07] 进制转换
来源：http://stj.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mqr.tarul.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://loq.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vwd.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wcd.yanxiufei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oko.xingfuxueyuan.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xvw.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bad.yangfankeji.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bmu.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://erm.redwolf501.top

Py:   pickle.dumps(obj)
来源：http://ifg.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fef.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://btb.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://duy.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rkg.jqgufenzy.top

Go:   encoding/gob
来源：http://odi.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://pfn.kuanghao11.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fkk.ppjwa.cn

================================================================================
来源：http://rcl.hammf.cn

L. 网络请求
来源：http://igk.xinyue.icu

================================================================================
来源：http://nci.zhengqikj.top

[L01] 发送 GET 请求
来源：http://ads.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jgh.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qgn.yj20258888.top

JS:   await fetch(url)
来源：http://sal.jqgufenzy.top

TS:   await fetch(url)
来源：http://bao.cheryme.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yab.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://nsd.hysaishi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gzu.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ucz.nanxuanxn.top

[L02] 发送 POST JSON
来源：http://gja.cqqwz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ybd.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qfe.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://epc.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kvq.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://leh.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kxz.gotoacloud.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jbj.jinghuilouyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pnm.zhoulong.xyz

[L03] 设置自定义请求头
来源：http://gfh.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jed.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wgs.xinyue.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yqf.yj20258888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ode.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jii.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ulk.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://voe.hesvh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vew.epnwcf.com

[L04] 设置超时
来源：http://qgr.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://ltz.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mbd.pycfn.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mda.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hud.hongshengwenyu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://utw.jianghu66.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qwf.quarkkingdee.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hdi.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bkr.pycfn.com

[L05] 上传文件（multipart）
来源：http://hpj.tian-w.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xhv.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lvt.yuanzhike.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mfk.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aka.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ogz.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kut.ydzc1.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://etx.chenlongwang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ivz.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://yah.ehwqpu.com

Py:   resp.json()
来源：http://lyx.tarul.cn

PHP:  json_decode($body, true);
来源：http://wnb.aizwys.cn

JS:   await resp.json()
来源：http://yny.yuanzhike.top

TS:   await resp.json()
来源：http://qbp.cheryme.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mlw.jianghu66.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ksn.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://rmw.yj20258.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://erm.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://slc.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tuh.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://els.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://ite.mhx1999.top

TS:   resp.ok;  resp.status
来源：http://tyg.jianghu66.top

Java: resp.statusCode()
来源：http://bcy.quarkkingdee.top

Go:   resp.StatusCode
来源：http://pps.gotoacloud.top

Ruby: resp.code.to_i
来源：http://dha.yanxiufei.cn

C#:   (int)resp.StatusCode
来源：http://bpe.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://pdn.nanxuanxn.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rou.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://hlz.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dhb.zycfv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tum.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tho.ivvv.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xhd.fzhhl.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dcd.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xck.jiagoushi.top

================================================================================
来源：http://acj.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://ymp.gzhubu.top

================================================================================
来源：http://dhl.mhx1999.top

[M01] 读取命令行参数
来源：http://wtb.c1oappe.top

Py:   sys.argv[1:]
来源：http://jyb.yanxiufei.cn

PHP:  $argv;  $argc;
来源：http://cfz.jlsjyb.cn

JS:   process.argv.slice(2)
来源：http://ilf.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://pfk.havefunace.top

Java: args 数组（main 方法参数）
来源：http://tlr.fzhhl.top

Go:   os.Args[1:]
来源：http://ucn.snrcjt.cn

Ruby: ARGV
来源：http://via.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://xvm.fengsongda.top

[M02] 读取环境变量
来源：http://xts.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://jpy.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rpo.svipenyu.cn

JS:   process.env.HOME
来源：http://bck.daxiang520.top

TS:   process.env.HOME
来源：http://lqu.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://ntb.yj202588.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wvk.bbcook.cn

Ruby: ENV["HOME"]
来源：http://ywg.hysaishi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cca.feifeiyinyue.top

[M03] 执行外部命令
来源：http://qot.yangfankeji.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lex.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rea.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lwi.jinyuanbaomall.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rtk.wangshuangyany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://erf.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ssa.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hwl.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://wuj.shanyushiyangkeji.top

[M04] 获取当前工作目录
来源：http://itn.ydzc1.top

Py:   os.getcwd()
来源：http://uph.yj20258.top

PHP:  getcwd();
来源：http://wgc.9152youxi.cn

JS:   process.cwd()
来源：http://evy.tanke756.top

TS:   process.cwd()
来源：http://wnf.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://mup.ydjk.org.cn

Go:   os.Getwd()
来源：http://odk.aibaodan.cn

Ruby: Dir.pwd
来源：http://evu.xziqi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fiw.bjfxy.top

[M05] 设置退出码
来源：http://hvj.vehdjk.com

Py:   sys.exit(1)
来源：http://kzf.yvedp.cn

PHP:  exit(1);
来源：http://xxn.shanyushiyangtech.top

JS:   process.exit(1)
来源：http://zjj.zhijiandao.cn

TS:   process.exit(1)
来源：http://zqo.daxiang520.top

Java: System.exit(1)
来源：http://hvp.fktsv.cn

Go:   os.Exit(1)
来源：http://oao.sweek.top

Ruby: exit 1
来源：http://gte.vqdsnc.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tsk.jianghu66.top

[M06] 向标准错误输出
来源：http://sks.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://uos.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gda.hcnkem.com

JS:   console.error("err")
来源：http://dut.ehwqpu.com

TS:   console.error("err")
来源：http://nmu.zycfv.cn

Java: System.err.println("err")
来源：http://ays.sjlbkw.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://buc.vehdjk.com

Ruby: warn "err"
来源：http://viw.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://iiw.zdqjudy.top

[M07] 判断是否为主入口
来源：http://aol.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://pgd.tanke756.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://itr.mhx1999.top

JS:   require.main === module
来源：http://kzz.cucudq.cn

TS:   require.main === module
来源：http://uxe.52xcode.cn

Java: public static void main(String[] args)
来源：http://kvk.hcnkem.com

Go:   func main()
来源：http://qdy.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://psd.bbcook.cn

C#:   static void Main(string[] args)
来源：http://hqj.hammf.cn

[M08] 获取系统与运行时信息
来源：http://fgw.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://cvv.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://gca.cashguo.top

JS:   process.platform;  process.version
来源：http://tuo.jinyuanbaomall.cn

TS:   process.platform;  process.version
来源：http://knz.hcnkem.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tvj.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bxx.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zwj.guowangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tuz.daria6918.cn

================================================================================
来源：http://woi.hnxiangtu.top

N. 数据结构与算法
来源：http://skd.bjfxy.top

================================================================================
来源：http://euw.gogol.net.cn

[N01] 二分查找（有序数组）
来源：http://ako.meibo888.top

Py:   bisect.bisect_left(arr, x)
来源：http://itc.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tmf.0kj1m.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://crc.jyoumei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vre.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://yim.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://eqy.yongpay.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://udw.yanxiufei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dtk.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://dru.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://rud.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aam.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qft.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jbp.ydzc1.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xyx.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://bsx.cucudq.cn

Ruby: arr.sort
来源：http://pzw.gogol.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cid.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://odz.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nul.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://shk.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gcu.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fju.zhiwuduotai.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uqz.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sxb.xuetiantiany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iwn.yongpay.top

C#:   // 手写递归，或 Array.Sort
来源：http://ben.cucudq.cn

[N04] 斐波那契数列
来源：http://wuk.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nqv.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dww.cheryme.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jkf.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rer.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://frk.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jqx.shanyushiyangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qra.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zbz.meibo888.top

[N05] 最大公约数
来源：http://mit.hongshengwenyu.top

Py:   math.gcd(a, b)
来源：http://big.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oli.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://olx.ppjwa.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cdb.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kxw.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://amy.cucudq.cn

Ruby: a.gcd(b)
来源：http://bwt.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pwa.guowangkeji.top

[N06] 判断回文字符串
来源：http://zgz.fengsongda.top

Py:   s == s[::-1]
来源：http://nsv.yj20258.top

PHP:  $s === strrev($s);
来源：http://vos.sjlbkw.cn

JS:   s === [...s].reverse().join("")
来源：http://fvf.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://toj.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bvq.vqdsnc.cn

Go:   // 双指针从两端比较
来源：http://ucc.iojbl.cn

Ruby: s == s.reverse
来源：http://sxt.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lac.xuanzx.com

[N07] 两数之和（返回下标）
来源：http://chc.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xuz.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fzj.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://iuu.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://zlh.316326.xyz

Java: // 手写 HashMap
来源：http://gzx.jinqigfzy.top

Go:   // 手写 map[int]int
来源：http://bpq.iojbl.cn

Ruby: // 手写 Hash
来源：http://iyy.cashguo.top

C#:   // 手写 Dictionary<int, int>
来源：http://dsd.cashguo.top

[N08] 生成全排列
来源：http://wtq.xinyue.icu


<!-- 参考信息 -->