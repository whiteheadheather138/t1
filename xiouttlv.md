代发 wailian999

[K02] JSON 字符串转对象
来源：http://bmv.gotoacloud.top

Py:   json.loads(s)
来源：http://gzz.shanyushiyangtech.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://anc.nwbrower.top

JS:   JSON.parse(s)
来源：http://qso.0kj1m.cn

TS:   JSON.parse(s)
来源：http://yhs.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ntb.hywenlv.cn

Go:   json.Unmarshal(data, &v)
来源：http://you.chenlongwang.top

Ruby: JSON.parse(s)
来源：http://ftb.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zqi.bbcook.cn

[K03] JSON 美化输出（带缩进）
来源：http://rsc.yj20258.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uue.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://elb.dianchejie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ttk.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gii.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kvp.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://clm.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://dll.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wyr.fzhhl.top

[K04] 读取 JSON 文件
来源：http://bmu.haohaochexian.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vqn.svipenyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yuc.ydzc1.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://otm.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hzp.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nqt.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tus.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vtx.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://opn.hywenlv.cn

[K05] 深拷贝对象
来源：http://onx.guannengcc.top

Py:   copy.deepcopy(obj)
来源：http://tov.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://jka.0kj1m.cn

JS:   structuredClone(obj)
来源：http://cmb.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://nmw.jqgufenzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cbz.svipenyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lbo.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://spj.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://crl.ywan-chungtsiang.top

[K06] 解析 URL 查询串
来源：http://wtp.hnxiangtu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tey.xingfuxueyuan.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hhb.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ppl.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pai.nanxinkj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bwz.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://beo.xuetiantiany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://crg.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gqn.birdmap.top

[K07] 进制转换
来源：http://orx.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mnv.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fik.fzhhl.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://anj.snrcjt.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xae.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hsm.fanxiaobao.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fso.shangyingyoupin.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sbr.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://anc.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://qpk.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://cxv.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pcv.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://tgx.bbcook.cn

TS:   v8.serialize(obj)        // Node
来源：http://win.xingfuxueyuan.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eue.xinyue.icu

Go:   encoding/gob
来源：http://yfx.xziqi.cn

Ruby: Marshal.dump(obj)
来源：http://ncy.haohaochexian.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://szy.sxryk.cn

================================================================================
来源：http://ods.gzhubu.top

L. 网络请求
来源：http://ujd.jlsjyb.cn

================================================================================
来源：http://qdm.yvedp.cn

[L01] 发送 GET 请求
来源：http://lla.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iiy.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://utv.snrcjt.cn

JS:   await fetch(url)
来源：http://csf.nwbrower.top

TS:   await fetch(url)
来源：http://jez.tianlin.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dxf.zycfv.cn

Go:   resp, err := http.Get(url)
来源：http://esl.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bii.shzxlz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://njz.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://msm.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mpw.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zpy.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qrz.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qkw.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wvo.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xkq.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rkw.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bsq.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://pnk.vqdsnc.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mwh.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vhy.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ndq.svipenyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bxy.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fey.sufxvd.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dbc.cdnleiting.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uce.fengsongda.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lqh.snrcjt.cn

[L04] 设置超时
来源：http://xqx.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://rjc.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bhf.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ooz.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sip.bbcook.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eqs.shanyushiyangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lrx.quarkkingdee.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nve.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://szv.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://poy.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jib.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pbm.wangdashe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ucg.zycfv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zyh.yangfankeji.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fbh.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wib.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rti.gogol.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mfh.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://zxe.zhengqikj.top

Py:   resp.json()
来源：http://toi.hongshengwenyu.top

PHP:  json_decode($body, true);
来源：http://yru.cashguo.top

JS:   await resp.json()
来源：http://cjh.feifeiyinyue.top

TS:   await resp.json()
来源：http://pnc.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uuj.shzxlz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yvk.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://mrd.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jji.ctjpmb.com

[L07] 处理 HTTP 状态码
来源：http://one.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xfw.ehwqpu.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ser.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://ots.hongshengwenyu.top

TS:   resp.ok;  resp.status
来源：http://dme.fzhhl.top

Java: resp.statusCode()
来源：http://txi.fktsv.cn

Go:   resp.StatusCode
来源：http://qmf.chenjidiqi.icu

Ruby: resp.code.to_i
来源：http://euz.meibo888.top

C#:   (int)resp.StatusCode
来源：http://wwy.yuxming.cn

[L08] 并发请求多个地址
来源：http://mql.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sew.quarkkingdee.top

PHP:  curl_multi_init() 系列
来源：http://rli.vehdjk.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xdq.xinyue.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wlm.tianlin.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hkz.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jdb.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eyh.daxiang520.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fmb.guannengcc.top

================================================================================
来源：http://rbt.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://dee.gogol.net.cn

================================================================================
来源：http://bqh.bbcook.cn

[M01] 读取命令行参数
来源：http://dqp.ppjwa.cn

Py:   sys.argv[1:]
来源：http://xqt.fktsv.cn

PHP:  $argv;  $argc;
来源：http://jsm.jinqigufen.top

JS:   process.argv.slice(2)
来源：http://gji.zhiwuduotai.top

TS:   process.argv.slice(2)
来源：http://pzk.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://eas.ybcxt.top

Go:   os.Args[1:]
来源：http://jxi.zhaomingkeji.xyz

Ruby: ARGV
来源：http://mzy.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://oaf.zhaomingkeji.xyz

[M02] 读取环境变量
来源：http://kit.tarul.cn

Py:   os.environ.get("HOME")
来源：http://lmn.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://evl.sxryk.cn

JS:   process.env.HOME
来源：http://qqg.guowangkeji.top

TS:   process.env.HOME
来源：http://rbz.smart0.xyz

Java: System.getenv("HOME")
来源：http://bhr.yj202588.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qvu.tanke756.top

Ruby: ENV["HOME"]
来源：http://cld.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lkr.snrcjt.cn

[M03] 执行外部命令
来源：http://ojo.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zcw.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xkp.vehdjk.com

JS:   child_process.execSync("ls -l").toString()
来源：http://djx.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vyp.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fny.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gzm.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jpo.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://izs.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://oua.jinqigfzy.top

Py:   os.getcwd()
来源：http://ste.hywenlv.cn

PHP:  getcwd();
来源：http://ybx.gogol.net.cn

JS:   process.cwd()
来源：http://itj.xziqi.cn

TS:   process.cwd()
来源：http://kdz.daxiang520.top

Java: Path.of("").toAbsolutePath()
来源：http://qbe.fktsv.cn

Go:   os.Getwd()
来源：http://hqh.chenzaomai.com

Ruby: Dir.pwd
来源：http://tej.xingfuxueyuan.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://lfj.daxiang520.top

[M05] 设置退出码
来源：http://phg.nanxinkj.top

Py:   sys.exit(1)
来源：http://buc.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://ext.xuanzx.com

JS:   process.exit(1)
来源：http://cts.vqdsnc.cn

TS:   process.exit(1)
来源：http://qap.nanxinkj.top

Java: System.exit(1)
来源：http://zgp.cheryme.top

Go:   os.Exit(1)
来源：http://rzs.cucudq.cn

Ruby: exit 1
来源：http://ogd.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://org.sufxvd.cn

[M06] 向标准错误输出
来源：http://bsu.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://wkr.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ndd.nanxinkj.top

JS:   console.error("err")
来源：http://lco.aibaodan.cn

TS:   console.error("err")
来源：http://uhz.xinyue.icu

Java: System.err.println("err")
来源：http://fzy.bjfxy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zah.cashguo.top

Ruby: warn "err"
来源：http://voj.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://qkz.ppjwa.cn

[M07] 判断是否为主入口
来源：http://lpx.quarkkingdee.top

Py:   if __name__ == "__main__":
来源：http://bqs.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eby.jinyuanbaomall.cn

JS:   require.main === module
来源：http://jnp.yueranfly.top

TS:   require.main === module
来源：http://jhp.9152youxi.cn

Java: public static void main(String[] args)
来源：http://hfb.jqgufenzy.top

Go:   func main()
来源：http://khj.sufxvd.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jti.yj20258.top

C#:   static void Main(string[] args)
来源：http://zem.fktsv.cn

[M08] 获取系统与运行时信息
来源：http://fre.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://pcs.guannengcc.top

PHP:  PHP_OS;  phpversion();
来源：http://yjp.yfazqb.com

JS:   process.platform;  process.version
来源：http://blk.zhixingplan.top

TS:   process.platform;  process.version
来源：http://mit.zhaomingkeji.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cfb.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pyf.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hba.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pga.shanyushiyangkeji.top

================================================================================
来源：http://cnd.tianlin.xyz

N. 数据结构与算法
来源：http://xem.hcnkem.com

================================================================================
来源：http://xgx.havefunace.top

[N01] 二分查找（有序数组）
来源：http://jez.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://wtt.cdnleiting.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xgz.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nur.epnwcf.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ons.haohaochexian.top

Java: Arrays.binarySearch(arr, x)
来源：http://chb.ywan-chungtsiang.top

Go:   sort.SearchInts(arr, x)
来源：http://uiy.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xim.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://iyg.jinqigfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://lvn.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://txm.redwolf501.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ypo.meibo888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://srm.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://lbg.fzhhl.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kpx.shuidangran.top

Go:   slices.Sort(arr)
来源：http://mok.sxryk.cn

Ruby: arr.sort
来源：http://ohd.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mut.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://isl.jianghu66.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dss.birdmap.top

PHP:  // 递归实现，或用 usort
来源：http://pbn.shuidangran.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vil.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oko.fzhhl.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://shf.yonumen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zea.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wwh.pengpengdd.cyou

C#:   // 手写递归，或 Array.Sort
来源：http://tmg.gotoacloud.top

[N04] 斐波那契数列
来源：http://xav.sufxvd.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://loj.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rdj.jyoumei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sfa.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sdi.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fvn.chenlongwang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fzw.vehdjk.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bod.yvedp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gom.wangshuangyany.cn

[N05] 最大公约数
来源：http://puh.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://aph.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jch.ctjpmb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gjk.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sjx.wangdashe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rjk.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://upn.jiagoushi.top

Ruby: a.gcd(b)
来源：http://ysa.ydzc1.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://azo.haohaochexian.top

[N06] 判断回文字符串
来源：http://kwi.ppjwa.cn

Py:   s == s[::-1]
来源：http://lsf.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://kxz.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://rro.zhiwuduotai.top

TS:   s === [...s].reverse().join("")
来源：http://uwa.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jgy.jqgufenzy.top

Go:   // 双指针从两端比较
来源：http://ewd.sufxvd.cn

Ruby: s == s.reverse
来源：http://szk.yuxming.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vmy.xylfe.cn

[N07] 两数之和（返回下标）
来源：http://clq.guowangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hww.haohaochexian.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://abz.yfazqb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://zqq.daxiang520.top

TS:   // 手写 Map<string, number>
来源：http://aus.wangdashe.top

Java: // 手写 HashMap
来源：http://edb.zycfv.cn

Go:   // 手写 map[int]int
来源：http://dbj.aizwys.cn

Ruby: // 手写 Hash
来源：http://zbo.shangyingyoupin.top

C#:   // 手写 Dictionary<int, int>
来源：http://vhs.aibaodan.cn

[N08] 生成全排列
来源：http://ejo.fzhhl.top

Py:   itertools.permutations(arr)
来源：http://xwr.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://gdr.jiagoushi.top

JS:   // 手写回溯递归
来源：http://htq.zycfv.cn

TS:   // 手写回溯递归
来源：http://edn.9152youxi.cn

Java: // 手写回溯递归
来源：http://taq.haohaochexian.top

Go:   // 手写回溯递归
来源：http://yog.9152youxi.cn

Ruby: arr.permutation.to_a
来源：http://jcy.pycfn.com

C#:   // 手写回溯递归
来源：http://gdv.shanyushiyangtech.top

[N09] 栈与队列
来源：http://xwb.gzhubu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ckz.jyoumei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mls.hnxiangtu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fkn.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jvu.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://esg.yanxiufei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nbn.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://muk.feifeiyinyue.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://frt.hnqzz.top

[N10] 链表节点定义
来源：http://cmt.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uli.cqqwz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jrd.nanxuanxn.top


<!-- 参考信息 -->