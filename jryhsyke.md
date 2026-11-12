代发 wailian999

================================================================================
来源：http://scg.c1oappe.top

K. JSON 与序列化
来源：http://dtk.xziqi.cn

================================================================================
来源：http://txm.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://nfc.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pny.pengpengdd.cyou

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ssx.zhengqikj.top

JS:   JSON.stringify(obj)
来源：http://ekp.xylfe.cn

TS:   JSON.stringify(obj)
来源：http://zmk.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fhw.cucudq.cn

Go:   json.Marshal(obj)
来源：http://nno.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ohj.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://isl.fengsongda.top

[K02] JSON 字符串转对象
来源：http://xji.zdbjq.cn

Py:   json.loads(s)
来源：http://okm.ydzc1.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ybc.hcnkem.com

JS:   JSON.parse(s)
来源：http://tjp.bjfxy.top

TS:   JSON.parse(s)
来源：http://yza.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ncs.zdqjudy.top

Go:   json.Unmarshal(data, &v)
来源：http://zoo.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://zns.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ymz.quarkkingdee.top

[K03] JSON 美化输出（带缩进）
来源：http://ero.yuxming.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vxy.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yfe.daria6918.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yfw.hammf.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://evv.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vjg.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zjz.xinyue.icu

Ruby: JSON.pretty_generate(obj)
来源：http://pev.ivvv.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rsb.cucudq.cn

[K04] 读取 JSON 文件
来源：http://flu.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vlq.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oth.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sdg.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gjv.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wsv.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://akh.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qsq.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yah.sysykeji.top

[K05] 深拷贝对象
来源：http://sau.ppjwa.cn

Py:   copy.deepcopy(obj)
来源：http://ztu.kuanghao11.cn

PHP:  unserialize(serialize($obj));
来源：http://yqt.zhengqikj.top

JS:   structuredClone(obj)
来源：http://vjw.yuanzhike.top

TS:   structuredClone(obj)
来源：http://oou.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://lcv.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cdb.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jmc.hcnkem.com

C#:   // 序列化往返，或自定义 Clone
来源：http://umm.hongshengwenyu.top

[K06] 解析 URL 查询串
来源：http://tty.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xvt.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hwl.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ujk.chenzaomai.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://egh.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fpv.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://avh.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wfc.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dcz.sxryk.cn

[K07] 进制转换
来源：http://hmz.vehdjk.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://khc.jlsjyb.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ejr.sufxvd.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mji.shuidangran.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jxo.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bds.zdqjudy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lcz.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://svm.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ptw.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://zaq.kuanghao11.cn

Py:   pickle.dumps(obj)
来源：http://rxb.yuanzhike.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jrt.cashguo.top

JS:   v8.serialize(obj)        // Node
来源：http://wrm.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://rry.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kac.xinyue.icu

Go:   encoding/gob
来源：http://hga.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://rjp.fanxiaobao.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://twf.pengpengdd.cyou

================================================================================
来源：http://raw.snrcjt.cn

L. 网络请求
来源：http://dyk.mhx1999.top

================================================================================
来源：http://ihr.cashguo.top

[L01] 发送 GET 请求
来源：http://rhv.hfpthk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vfg.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kev.cucudq.cn

JS:   await fetch(url)
来源：http://dhi.shangyingyoupin.top

TS:   await fetch(url)
来源：http://aiv.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wxn.chenjidiqi.icu

Go:   resp, err := http.Get(url)
来源：http://mnc.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eub.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qtf.yj20258.top

[L02] 发送 POST JSON
来源：http://ire.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://drg.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zvt.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vwe.sjlbkw.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lvw.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hwg.zdbjq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://css.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://twc.guannengcc.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zkd.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://ifz.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jqh.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zpb.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pwq.epnwcf.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://miy.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bwj.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nzv.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uop.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://szx.shzxlz.cn

[L04] 设置超时
来源：http://csc.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://bab.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://men.haohaochexian.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lfw.jiagoushi.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aif.shangyingyoupin.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yme.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jfn.tian-w.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://the.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hmu.wangdashe.top

[L05] 上传文件（multipart）
来源：http://jdq.iojbl.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://skh.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kcs.wangshuangyany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rxl.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lvm.zhengqikj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ngj.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://alm.9152youxi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kyy.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kjn.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://gmf.jiagoushi.top

Py:   resp.json()
来源：http://ghh.xingfuxueyuan.xyz

PHP:  json_decode($body, true);
来源：http://jsm.xinyue.icu

JS:   await resp.json()
来源：http://xin.316326.xyz

TS:   await resp.json()
来源：http://mvf.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fnf.yj20258888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cuq.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://dfj.quarkkingdee.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hsz.sjlbkw.cn

[L07] 处理 HTTP 状态码
来源：http://ggx.quarkkingdee.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://keu.chenlongwang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://omq.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://xss.zycfv.cn

TS:   resp.ok;  resp.status
来源：http://zkd.dianchejie.cn

Java: resp.statusCode()
来源：http://wkf.sxryk.cn

Go:   resp.StatusCode
来源：http://bdr.zhengqikj.top

Ruby: resp.code.to_i
来源：http://dlu.yj202588.top

C#:   (int)resp.StatusCode
来源：http://sdp.hysaishi.cn

[L08] 并发请求多个地址
来源：http://kda.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://miz.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://zwr.gogol.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qbm.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cpo.hnqzz.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kdj.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://swk.nanxuanxn.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qxh.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hgu.zhixingplan.top

================================================================================
来源：http://ftc.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://egv.hongshengwenyu.top

================================================================================
来源：http://kat.ppjwa.cn

[M01] 读取命令行参数
来源：http://sac.svipenyu.cn

Py:   sys.argv[1:]
来源：http://cor.ivvv.top

PHP:  $argv;  $argc;
来源：http://vub.zycfv.cn

JS:   process.argv.slice(2)
来源：http://rfa.redwolf501.top

TS:   process.argv.slice(2)
来源：http://phc.uphjek.com

Java: args 数组（main 方法参数）
来源：http://qbv.zdbjq.cn

Go:   os.Args[1:]
来源：http://pyx.sweek.top

Ruby: ARGV
来源：http://mcg.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://lum.dashuyun.cn

[M02] 读取环境变量
来源：http://wyh.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://myj.jianghu66.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gog.cucudq.cn

JS:   process.env.HOME
来源：http://bwh.snrcjt.cn

TS:   process.env.HOME
来源：http://vdt.hnqzz.top

Java: System.getenv("HOME")
来源：http://tlc.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oem.yj20258888.top

Ruby: ENV["HOME"]
来源：http://trq.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ksv.jianghu66.top

[M03] 执行外部命令
来源：http://hyt.zdbjq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xry.meibo888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qbf.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dkp.hywenlv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mle.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jjh.dashuyun.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tbf.bjfxy.top

Ruby: system("ls -l");  `ls -l`
来源：http://cue.pycfn.com

C#:   Process.Start("ls", "-l");
来源：http://rfj.ybcxt.top

[M04] 获取当前工作目录
来源：http://cle.yongpay.top

Py:   os.getcwd()
来源：http://zqw.zhengqikj.top

PHP:  getcwd();
来源：http://hno.svipenyu.cn

JS:   process.cwd()
来源：http://vxg.yuanzhike.top

TS:   process.cwd()
来源：http://gbl.ivvv.top

Java: Path.of("").toAbsolutePath()
来源：http://jzb.quarkkingdee.top

Go:   os.Getwd()
来源：http://kln.epnwcf.com

Ruby: Dir.pwd
来源：http://jqw.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://tsd.sweek.top

[M05] 设置退出码
来源：http://uug.cqqwz.cn

Py:   sys.exit(1)
来源：http://oho.zdqjudy.top

PHP:  exit(1);
来源：http://bxg.sjlbkw.cn

JS:   process.exit(1)
来源：http://xiu.yangfankeji.com

TS:   process.exit(1)
来源：http://wjx.guowangkeji.top

Java: System.exit(1)
来源：http://ult.yuxming.cn

Go:   os.Exit(1)
来源：http://yil.hcnkem.com

Ruby: exit 1
来源：http://ymc.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oxq.yvedp.cn

[M06] 向标准错误输出
来源：http://kcr.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://lky.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eiv.vqdsnc.cn

JS:   console.error("err")
来源：http://ffq.ppjwa.cn

TS:   console.error("err")
来源：http://uza.ivvv.top

Java: System.err.println("err")
来源：http://rah.bjfxy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bsd.shzxlz.cn

Ruby: warn "err"
来源：http://fxi.ybcxt.top

C#:   Console.Error.WriteLine("err")
来源：http://xyb.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://pro.jinyuanbaomall.cn

Py:   if __name__ == "__main__":
来源：http://qiw.svipenyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xgz.yongpay.top

JS:   require.main === module
来源：http://bcx.dashuyun.cn

TS:   require.main === module
来源：http://oya.hcnkem.com

Java: public static void main(String[] args)
来源：http://pyg.ybcxt.top

Go:   func main()
来源：http://kxi.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wwx.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://vsm.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://pff.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://jxs.yvedp.cn

PHP:  PHP_OS;  phpversion();
来源：http://kbe.hywenlv.cn

JS:   process.platform;  process.version
来源：http://pvu.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://mpk.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cxh.hongshengwenyu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gzv.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oui.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://atr.iojbl.cn

================================================================================
来源：http://jdj.cqqwz.cn

N. 数据结构与算法
来源：http://eku.fehbvm.com

================================================================================
来源：http://mui.xinyue.icu

[N01] 二分查找（有序数组）
来源：http://uvd.zhaomingkeji.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://jat.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wam.zhongyouzk.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aou.iojbl.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dpc.xuetiantiany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kym.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://xfc.jinqigfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xzb.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nwg.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://vzf.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://dko.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ckh.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://bxl.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bjs.shzxlz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tuk.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://eiw.yuanzhike.top

Ruby: arr.sort
来源：http://ase.daria6918.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://aky.yonumen.top

[N03] 快速排序（分治示例）
来源：http://fuh.yanxiufei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dit.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://caq.jyoumei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cju.wangshuangyany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mds.yj20258.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rrj.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://znt.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wwg.jqgufenzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://egp.jinyuanbaomall.cn

[N04] 斐波那契数列
来源：http://cnp.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aao.xinyue.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zgj.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jbh.ivvv.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://emu.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fby.xylfe.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tid.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hdo.xylfe.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mcf.dashuyun.cn

[N05] 最大公约数
来源：http://bcd.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://wzi.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bvx.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jba.nanxinkj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uwu.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ymv.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lov.cucudq.cn

Ruby: a.gcd(b)
来源：http://bio.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://its.sysykeji.top

[N06] 判断回文字符串
来源：http://eyr.cheryme.top

Py:   s == s[::-1]
来源：http://lsf.zdqjudy.top

PHP:  $s === strrev($s);
来源：http://ewl.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://oxc.zdqjudy.top

TS:   s === [...s].reverse().join("")
来源：http://xqi.nanxinkj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fsv.yfazqb.com

Go:   // 双指针从两端比较
来源：http://nnu.fzhhl.top

Ruby: s == s.reverse
来源：http://pnj.yj20258.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://inj.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://qkd.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://twq.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tmv.hcnkem.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ous.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://xuk.yueranfly.top

Java: // 手写 HashMap
来源：http://qfw.nanxuanxn.top

Go:   // 手写 map[int]int
来源：http://kdh.dashuyun.cn

Ruby: // 手写 Hash
来源：http://jhl.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qsc.yonumen.top

[N08] 生成全排列
来源：http://zho.zdbjq.cn

Py:   itertools.permutations(arr)
来源：http://cus.0kj1m.cn

PHP:  // 手写递归交换
来源：http://fbn.aizwys.cn

JS:   // 手写回溯递归
来源：http://uzo.zdqjudy.top

TS:   // 手写回溯递归
来源：http://fhb.xylfe.cn

Java: // 手写回溯递归
来源：http://yhp.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://peh.dashuyun.cn

Ruby: arr.permutation.to_a
来源：http://txv.bjfxy.top

C#:   // 手写回溯递归
来源：http://ebn.yvedp.cn


<!-- 参考信息 -->