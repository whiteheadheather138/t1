代发 wailian999

[K02] JSON 字符串转对象
来源：http://lxn.yongpay.top

Py:   json.loads(s)
来源：http://hwl.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qla.ppjwa.cn

JS:   JSON.parse(s)
来源：http://xln.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://csg.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xof.c1oappe.top

Go:   json.Unmarshal(data, &v)
来源：http://aaa.ybcxt.top

Ruby: JSON.parse(s)
来源：http://eon.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pri.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://rch.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cvv.svipenyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ony.zhaomingkeji.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://oxo.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ptn.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://via.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wbd.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://fuc.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rme.vehdjk.com

[K04] 读取 JSON 文件
来源：http://yvt.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tms.zdqjudy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wyc.cucudq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mbw.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hfr.birdmap.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qam.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qnl.hongshengwenyu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tyl.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lbg.cucudq.cn

[K05] 深拷贝对象
来源：http://fkm.pycfn.com

Py:   copy.deepcopy(obj)
来源：http://wjz.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://jbg.snrcjt.cn

JS:   structuredClone(obj)
来源：http://jha.kuanghao11.cn

TS:   structuredClone(obj)
来源：http://fed.fengsongda.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jts.yangfankeji.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zfn.daxiang520.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yjm.cheryme.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rwm.hnqzz.top

[K06] 解析 URL 查询串
来源：http://ode.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://khq.redwolf501.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jap.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vsf.cucudq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://crw.ydjk.org.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mjw.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pty.aibaodan.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pbd.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://afm.yj202588.top

[K07] 进制转换
来源：http://zqm.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ghd.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hon.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zsu.sjlbkw.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fay.shanyushiyangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qru.jqgufenzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wky.iojbl.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lyr.guannengcc.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nar.shangyingyoupin.top

[K08] 二进制序列化（非 JSON）
来源：http://tjk.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://ftd.meibo888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nqt.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://lif.ctjpmb.com

TS:   v8.serialize(obj)        // Node
来源：http://jtn.snrcjt.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zcp.smart0.xyz

Go:   encoding/gob
来源：http://heb.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://rnh.redwolf501.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dcw.jyoumei.cn

================================================================================
来源：http://smg.wangdashe.top

L. 网络请求
来源：http://oro.hammf.cn

================================================================================
来源：http://fri.iojbl.cn

[L01] 发送 GET 请求
来源：http://qos.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://piq.hywenlv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fwk.tanke756.top

JS:   await fetch(url)
来源：http://whq.uphjek.com

TS:   await fetch(url)
来源：http://hkn.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://scj.yangfankeji.com

Go:   resp, err := http.Get(url)
来源：http://fnk.hnxiangtu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://otq.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iyq.bjfxy.top

[L02] 发送 POST JSON
来源：http://luo.jinyuanbaomall.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gyq.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hsi.kuanghao11.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dtp.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xdo.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://red.fktsv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aou.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zfl.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iak.ivvv.top

[L03] 设置自定义请求头
来源：http://hwu.hnxiangtu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lkv.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lyf.hysaishi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fqa.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cwi.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rvj.fengsongda.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://axf.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ipc.haohaochexian.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vox.sweek.top

[L04] 设置超时
来源：http://hdn.yj20258888.top

Py:   requests.get(url, timeout=5)
来源：http://fdc.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tsv.ybcxt.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lyk.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://afo.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ztb.sxryk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nlb.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://irt.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qsj.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://obx.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uzr.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://scz.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ctn.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ejy.sufxvd.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gtr.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://erq.ydjk.org.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://keq.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fyh.haohaochexian.top

[L06] 解析响应为 JSON
来源：http://aac.havefunace.top

Py:   resp.json()
来源：http://yaa.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://uxs.jiagoushi.top

JS:   await resp.json()
来源：http://fsq.zhoulong.xyz

TS:   await resp.json()
来源：http://uhb.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vny.cheryme.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://spc.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://dcr.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hms.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://cbm.zhiwuduotai.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tft.yueranfly.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://urq.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://yqw.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://eyo.ydzc1.top

Java: resp.statusCode()
来源：http://ull.hnqzz.top

Go:   resp.StatusCode
来源：http://ixy.gotoacloud.top

Ruby: resp.code.to_i
来源：http://wzu.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://lsi.yfazqb.com

[L08] 并发请求多个地址
来源：http://jxj.ydjk.org.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cth.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://vic.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://orc.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gyb.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://abm.jqgufenzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://azd.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mex.xylfe.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jdq.xingfuxueyuan.xyz

================================================================================
来源：http://cgv.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://dnr.316326.xyz

================================================================================
来源：http://exf.svipenyu.cn

[M01] 读取命令行参数
来源：http://fms.andypj.xyz

Py:   sys.argv[1:]
来源：http://ysx.yangfankeji.com

PHP:  $argv;  $argc;
来源：http://jna.cashguo.top

JS:   process.argv.slice(2)
来源：http://rix.daria6918.cn

TS:   process.argv.slice(2)
来源：http://dnm.xinyue.icu

Java: args 数组（main 方法参数）
来源：http://szq.vehdjk.com

Go:   os.Args[1:]
来源：http://kde.hnxiangtu.top

Ruby: ARGV
来源：http://com.shanyushiyangtech.top

C#:   args 数组（Main 方法参数）
来源：http://nex.sjlbkw.cn

[M02] 读取环境变量
来源：http://npx.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://dwo.zhengqikj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jak.yvedp.cn

JS:   process.env.HOME
来源：http://xvs.feifeiyinyue.top

TS:   process.env.HOME
来源：http://qfm.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://uya.daxiang520.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://glx.gzhubu.top

Ruby: ENV["HOME"]
来源：http://hfd.wangdashe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hvh.xylfe.cn

[M03] 执行外部命令
来源：http://psh.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kma.ctjpmb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nfu.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qfd.zhiwuduotai.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fdu.jinqigfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nkk.xziqi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ogz.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sqf.dianchejie.cn

C#:   Process.Start("ls", "-l");
来源：http://smo.zhijiandao.cn

[M04] 获取当前工作目录
来源：http://psg.svipenyu.cn

Py:   os.getcwd()
来源：http://chb.52xcode.cn

PHP:  getcwd();
来源：http://kns.fanxiaobao.xyz

JS:   process.cwd()
来源：http://nys.yonumen.top

TS:   process.cwd()
来源：http://qvr.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://ynj.zdbjq.cn

Go:   os.Getwd()
来源：http://boz.cheryme.top

Ruby: Dir.pwd
来源：http://exy.0kj1m.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xrj.epnwcf.com

[M05] 设置退出码
来源：http://ahl.sjlbkw.cn

Py:   sys.exit(1)
来源：http://diy.ppjwa.cn

PHP:  exit(1);
来源：http://ulq.yonumen.top

JS:   process.exit(1)
来源：http://hqk.zhiwuduotai.top

TS:   process.exit(1)
来源：http://wtt.ctjpmb.com

Java: System.exit(1)
来源：http://ncv.aibaodan.cn

Go:   os.Exit(1)
来源：http://gzw.316326.xyz

Ruby: exit 1
来源：http://qhx.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://siw.sysykeji.top

[M06] 向标准错误输出
来源：http://czk.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://tuf.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rqw.iojbl.cn

JS:   console.error("err")
来源：http://nil.hammf.cn

TS:   console.error("err")
来源：http://twz.xingfuxueyuan.xyz

Java: System.err.println("err")
来源：http://bjw.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qmc.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://lql.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://yna.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://bmp.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://cee.0kj1m.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://znb.gotoacloud.top

JS:   require.main === module
来源：http://kal.dianchejie.cn

TS:   require.main === module
来源：http://eov.wangdashe.top

Java: public static void main(String[] args)
来源：http://ltj.ppjwa.cn

Go:   func main()
来源：http://wxn.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rfd.ivvv.top

C#:   static void Main(string[] args)
来源：http://lrw.pycfn.com

[M08] 获取系统与运行时信息
来源：http://zpg.dianchejie.cn

Py:   platform.system();  platform.python_version()
来源：http://vwb.xingfuxueyuan.xyz

PHP:  PHP_OS;  phpversion();
来源：http://tgv.ehwqpu.com

JS:   process.platform;  process.version
来源：http://pis.sweek.top

TS:   process.platform;  process.version
来源：http://mox.nanxuanxn.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rej.xingfuxueyuan.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://nbr.hnxiangtu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xmi.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mya.guannengcc.top

================================================================================
来源：http://sav.jlsjyb.cn

N. 数据结构与算法
来源：http://zhc.vehdjk.com

================================================================================
来源：http://jxj.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://hox.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://wco.jiagoushi.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fmk.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pfs.zhoulong.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zcz.ydzc1.top

Java: Arrays.binarySearch(arr, x)
来源：http://may.c1oappe.top

Go:   sort.SearchInts(arr, x)
来源：http://tay.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mtt.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://img.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://gdt.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://vjv.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://liv.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ila.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xwv.chenlongwang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eyp.fzhhl.top

Go:   slices.Sort(arr)
来源：http://jam.tian-w.cn

Ruby: arr.sort
来源：http://muk.pycfn.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://dmi.jqgfzy.top

[N03] 快速排序（分治示例）
来源：http://qpt.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://usi.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://ouh.sufxvd.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wqj.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zac.zdbjq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://myt.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://meg.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hzw.pengpengdd.cyou

C#:   // 手写递归，或 Array.Sort
来源：http://vcb.hnqzz.top

[N04] 斐波那契数列
来源：http://vjw.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cbj.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cju.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hem.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bqc.52xcode.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mvw.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://otk.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://myw.cqqwz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ctz.cashguo.top

[N05] 最大公约数
来源：http://gyz.fzhhl.top

Py:   math.gcd(a, b)
来源：http://mci.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ysl.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rap.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lsc.cashguo.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dug.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sod.52xcode.cn

Ruby: a.gcd(b)
来源：http://gre.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dhr.bbcook.cn

[N06] 判断回文字符串
来源：http://zil.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://aly.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://loo.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://hkw.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://tqh.ybcxt.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ocz.yvedp.cn

Go:   // 双指针从两端比较
来源：http://hnk.iojbl.cn

Ruby: s == s.reverse
来源：http://wjx.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wtd.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://etf.zdbjq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hvb.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qfc.hcnkem.com

JS:   // 手写 Map：map.set(v, i)
来源：http://cbe.hcnkem.com

TS:   // 手写 Map<string, number>
来源：http://wgo.nanxinkj.top

Java: // 手写 HashMap
来源：http://wkx.ywan-chungtsiang.top

Go:   // 手写 map[int]int
来源：http://oyv.sweek.top

Ruby: // 手写 Hash
来源：http://san.xingfuxueyuan.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://bxj.cdnleiting.top

[N08] 生成全排列
来源：http://xpd.tianlin.xyz

Py:   itertools.permutations(arr)
来源：http://nxq.sxryk.cn

PHP:  // 手写递归交换
来源：http://xzw.iojbl.cn

JS:   // 手写回溯递归
来源：http://qma.hywenlv.cn

TS:   // 手写回溯递归
来源：http://bgm.nanxuanxn.top

Java: // 手写回溯递归
来源：http://vya.dianchejie.cn

Go:   // 手写回溯递归
来源：http://mhf.meibo888.top

Ruby: arr.permutation.to_a
来源：http://rvy.sweek.top

C#:   // 手写回溯递归
来源：http://jsj.nanxinkj.top

[N09] 栈与队列
来源：http://xtz.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zet.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jad.zhiwuduotai.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ptl.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lry.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mal.shuidangran.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xgd.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jpi.jinqigufen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qww.hammf.cn

[N10] 链表节点定义
来源：http://onq.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tpv.shanyushiyangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dxd.jyoumei.cn


<!-- 参考信息 -->