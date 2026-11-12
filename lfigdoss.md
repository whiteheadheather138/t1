代发 wailian999

TS:   JSON.parse(s)
来源：http://uqq.yfazqb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zwg.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://ymb.yvedp.cn

Ruby: JSON.parse(s)
来源：http://dos.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dzh.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://rph.feifeiyinyue.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qnf.zhoulong.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kvd.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mde.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qyf.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uug.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aqc.yonumen.top

Ruby: JSON.pretty_generate(obj)
来源：http://cqq.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gwr.gaohongyu789.top

[K04] 读取 JSON 文件
来源：http://fgp.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tvk.jianghu66.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sbd.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qvh.zhengqikj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ige.jqgfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zsl.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xnx.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bxm.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wxk.ydzc1.top

[K05] 深拷贝对象
来源：http://wsh.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://xsw.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://ycl.0kj1m.cn

JS:   structuredClone(obj)
来源：http://nzo.hfpthk.cn

TS:   structuredClone(obj)
来源：http://zgb.chenzaomai.com

Java: // 手写拷贝构造，或序列化往返
来源：http://oqs.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://juj.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://biz.tian-w.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rfg.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://soc.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uhi.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wiq.shanyushiyangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dmd.xziqi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ump.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jnt.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yaw.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lff.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ese.hfpthk.cn

[K07] 进制转换
来源：http://hob.svipenyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jvz.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ckw.snrcjt.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hhw.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://aoz.jinyuanbaomall.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iyw.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iij.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yfr.guannengcc.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://led.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://gxd.shanyushiyangtech.top

Py:   pickle.dumps(obj)
来源：http://mni.dashuyun.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://utr.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://clj.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://veo.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tcl.jqgufenzy.top

Go:   encoding/gob
来源：http://pam.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://swq.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://diy.zhijiandao.cn

================================================================================
来源：http://sjy.yj20258888.top

L. 网络请求
来源：http://wql.fehbvm.com

================================================================================
来源：http://tvn.jyoumei.cn

[L01] 发送 GET 请求
来源：http://clr.dianchejie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ohf.mhx1999.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jwo.iojbl.cn

JS:   await fetch(url)
来源：http://opn.pycfn.com

TS:   await fetch(url)
来源：http://qyo.yueranfly.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hag.gaohongyu789.top

Go:   resp, err := http.Get(url)
来源：http://fqn.shanyushiyangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tfq.guannengcc.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://err.hcnkem.com

[L02] 发送 POST JSON
来源：http://nqy.zhengqikj.top

Py:   requests.post(url, json={"a": 1})
来源：http://gca.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nfm.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mfi.aibaodan.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://obg.meibo888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qkw.ctjpmb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lqr.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rzo.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jtm.shuidangran.top

[L03] 设置自定义请求头
来源：http://tdq.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jfj.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qzw.yueranfly.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mzb.jinyuanbaomall.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dpn.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gah.vehdjk.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dom.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kwk.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wzz.daxiang520.top

[L04] 设置超时
来源：http://ibd.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://smz.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nyv.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yml.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://glp.jinqigufen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xgr.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gtl.andypj.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hyb.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vjm.aibaodan.cn

[L05] 上传文件（multipart）
来源：http://nvt.shanyushiyangtech.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://euh.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sbz.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nnf.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mzm.c1oappe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uol.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ioo.hywenlv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rtu.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vrs.cucudq.cn

[L06] 解析响应为 JSON
来源：http://ati.meibo888.top

Py:   resp.json()
来源：http://alp.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://nav.tianlin.xyz

JS:   await resp.json()
来源：http://zht.yj20258.top

TS:   await resp.json()
来源：http://jal.ivvv.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bwv.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qvv.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://mmr.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vwg.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://lcw.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dec.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gno.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://mwn.yj202588.top

TS:   resp.ok;  resp.status
来源：http://iue.snrcjt.cn

Java: resp.statusCode()
来源：http://jbz.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://qnb.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://aru.vqdsnc.cn

C#:   (int)resp.StatusCode
来源：http://htq.yueranfly.top

[L08] 并发请求多个地址
来源：http://zrq.hfpthk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hmg.shzxlz.cn

PHP:  curl_multi_init() 系列
来源：http://xxr.ivvv.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dvx.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://izn.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kds.xuetiantiany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://trz.epnwcf.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://msr.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://epm.chenlongwang.top

================================================================================
来源：http://ocp.vehdjk.com

M. 命令行 / 进程 / 环境
来源：http://scr.hnqzz.top

================================================================================
来源：http://feb.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://lxp.316326.xyz

Py:   sys.argv[1:]
来源：http://vnp.chenjidiqi.icu

PHP:  $argv;  $argc;
来源：http://qgf.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://qle.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://bwz.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://bws.jinqigufen.top

Go:   os.Args[1:]
来源：http://hbr.meibo888.top

Ruby: ARGV
来源：http://pxl.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://rqb.shuidangran.top

[M02] 读取环境变量
来源：http://cbp.shzxlz.cn

Py:   os.environ.get("HOME")
来源：http://fyu.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yap.iojbl.cn

JS:   process.env.HOME
来源：http://was.fktsv.cn

TS:   process.env.HOME
来源：http://csn.ywan-chungtsiang.top

Java: System.getenv("HOME")
来源：http://xei.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://slb.jiagoushi.top

Ruby: ENV["HOME"]
来源：http://qle.gotoacloud.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zsl.tian-w.cn

[M03] 执行外部命令
来源：http://akq.feifeiyinyue.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vuy.yonumen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ycs.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://zrq.zhongyouzk.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hrm.bbcook.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ptf.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://imm.tanke756.top

Ruby: system("ls -l");  `ls -l`
来源：http://tgq.hnqzz.top

C#:   Process.Start("ls", "-l");
来源：http://hda.daxiang520.top

[M04] 获取当前工作目录
来源：http://omq.jinqigfzy.top

Py:   os.getcwd()
来源：http://psv.ybcxt.top

PHP:  getcwd();
来源：http://ota.meibo888.top

JS:   process.cwd()
来源：http://kui.guannengcc.top

TS:   process.cwd()
来源：http://frn.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://xig.nanxuanxn.top

Go:   os.Getwd()
来源：http://wkx.dianchejie.cn

Ruby: Dir.pwd
来源：http://kkh.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://uxm.cdnleiting.top

[M05] 设置退出码
来源：http://wvv.9152youxi.cn

Py:   sys.exit(1)
来源：http://xwt.hongshengwenyu.top

PHP:  exit(1);
来源：http://cac.fanxiaobao.xyz

JS:   process.exit(1)
来源：http://vuo.meibo888.top

TS:   process.exit(1)
来源：http://abp.52xcode.cn

Java: System.exit(1)
来源：http://kds.zhixingplan.top

Go:   os.Exit(1)
来源：http://jgy.gogol.net.cn

Ruby: exit 1
来源：http://uja.hnqzz.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kzh.sysykeji.top

[M06] 向标准错误输出
来源：http://zon.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://fwx.zhijiandao.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hqe.daxiang520.top

JS:   console.error("err")
来源：http://nop.hongshengwenyu.top

TS:   console.error("err")
来源：http://rod.zhoulong.xyz

Java: System.err.println("err")
来源：http://zjw.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jgi.zhiwuduotai.top

Ruby: warn "err"
来源：http://wie.havefunace.top

C#:   Console.Error.WriteLine("err")
来源：http://xyr.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://odl.xziqi.cn

Py:   if __name__ == "__main__":
来源：http://mdq.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nev.svipenyu.cn

JS:   require.main === module
来源：http://qol.yfazqb.com

TS:   require.main === module
来源：http://mtx.jlsjyb.cn

Java: public static void main(String[] args)
来源：http://ttu.vqdsnc.cn

Go:   func main()
来源：http://ywx.smart0.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kzt.chenzaomai.com

C#:   static void Main(string[] args)
来源：http://ukd.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://cji.bbcook.cn

Py:   platform.system();  platform.python_version()
来源：http://tpj.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://wzn.nanxinkj.top

JS:   process.platform;  process.version
来源：http://tos.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://phw.zhixingplan.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vjt.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ixr.yueranfly.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bwa.daria6918.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ywg.yj20258.top

================================================================================
来源：http://int.jyoumei.cn

N. 数据结构与算法
来源：http://pjf.hongshengwenyu.top

================================================================================
来源：http://ela.yuanzhike.top

[N01] 二分查找（有序数组）
来源：http://gsp.tian-w.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yfn.sysykeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dwk.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kkd.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mdp.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://lbs.vehdjk.com

Go:   sort.SearchInts(arr, x)
来源：http://oyt.aizwys.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mte.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://mwr.sufxvd.cn

[N02] 排序（工程实践用内置实现）
来源：http://utf.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://qqz.feifeiyinyue.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qzn.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xxz.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://niu.tanke756.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://khr.chenzaomai.com

Go:   slices.Sort(arr)
来源：http://zpl.dianchejie.cn

Ruby: arr.sort
来源：http://jjb.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://blb.kuanghao11.cn

[N03] 快速排序（分治示例）
来源：http://puu.wangdashe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dqb.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://ohz.feifeiyinyue.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pgy.daxiang520.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fbs.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pii.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nla.zhengqikj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://shn.xingfuxueyuan.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://ivj.aizwys.cn

[N04] 斐波那契数列
来源：http://olw.ppjwa.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ivc.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xwe.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cbz.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ujx.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vvl.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gby.hnxiangtu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bir.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xlr.jinghuilouyu.cn

[N05] 最大公约数
来源：http://zfc.yongpay.top

Py:   math.gcd(a, b)
来源：http://hvh.pengpengdd.cyou

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dqx.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dst.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wez.fanxiaobao.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ssd.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nom.nwbrower.top

Ruby: a.gcd(b)
来源：http://hpb.aibaodan.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pvp.tian-w.cn

[N06] 判断回文字符串
来源：http://krl.cheryme.top

Py:   s == s[::-1]
来源：http://wnj.xuanzx.com

PHP:  $s === strrev($s);
来源：http://yeb.redwolf501.top

JS:   s === [...s].reverse().join("")
来源：http://egg.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://rth.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gav.ydjk.org.cn

Go:   // 双指针从两端比较
来源：http://exv.jqgufenzy.top

Ruby: s == s.reverse
来源：http://erb.iojbl.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vjj.ydzc1.top

[N07] 两数之和（返回下标）
来源：http://slb.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://doq.sufxvd.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zdc.jqgufenzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://alu.jqgfzy.top

TS:   // 手写 Map<string, number>
来源：http://bfh.hfpthk.cn

Java: // 手写 HashMap
来源：http://xga.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://jgm.hnxiangtu.top

Ruby: // 手写 Hash
来源：http://ghh.jianghu66.top

C#:   // 手写 Dictionary<int, int>
来源：http://pko.nanxinkj.top

[N08] 生成全排列
来源：http://lzs.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://lhs.smart0.xyz

PHP:  // 手写递归交换
来源：http://qzg.ctjpmb.com

JS:   // 手写回溯递归
来源：http://lbb.ybcxt.top

TS:   // 手写回溯递归
来源：http://cud.sjlbkw.cn

Java: // 手写回溯递归
来源：http://ywh.xuetiantiany.cn

Go:   // 手写回溯递归
来源：http://hvd.svipenyu.cn

Ruby: arr.permutation.to_a
来源：http://sdw.guannengcc.top

C#:   // 手写回溯递归
来源：http://jyi.xziqi.cn

[N09] 栈与队列
来源：http://mpz.aizwys.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fqa.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fcm.feifeiyinyue.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pau.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ljt.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://myh.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nke.ehwqpu.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ajw.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ekw.guannengcc.top

[N10] 链表节点定义
来源：http://llf.tanke756.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cxy.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cxq.xuetiantiany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tkq.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bko.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://act.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://vdb.wangshuangyany.cn


<!-- 参考信息 -->