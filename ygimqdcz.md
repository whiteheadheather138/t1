代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://btg.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://faa.haohaochexian.top

JS:   JSON.stringify(obj)
来源：http://xap.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://lei.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://poo.fehbvm.com

Go:   json.Marshal(obj)
来源：http://koy.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://gpe.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://egj.fehbvm.com

[K02] JSON 字符串转对象
来源：http://dvt.feifeiyinyue.top

Py:   json.loads(s)
来源：http://eju.fktsv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cjl.zhengqikj.top

JS:   JSON.parse(s)
来源：http://pbl.xuanzx.com

TS:   JSON.parse(s)
来源：http://nor.aibaodan.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aze.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://sun.yvedp.cn

Ruby: JSON.parse(s)
来源：http://ihu.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rxj.xylfe.cn

[K03] JSON 美化输出（带缩进）
来源：http://gmh.vqdsnc.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qzv.shzxlz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tuf.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://dyn.epnwcf.com

TS:   JSON.stringify(obj, null, 2)
来源：http://enp.ctjpmb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iax.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jel.daxiang520.top

Ruby: JSON.pretty_generate(obj)
来源：http://jrf.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dkl.fehbvm.com

[K04] 读取 JSON 文件
来源：http://sbm.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://txf.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zfo.hnqzz.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ymt.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://svj.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jum.jyoumei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rpm.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fcv.tanke756.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kyg.daxiang520.top

[K05] 深拷贝对象
来源：http://cxn.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://mno.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://yrs.0kj1m.cn

JS:   structuredClone(obj)
来源：http://yww.yuanzhike.top

TS:   structuredClone(obj)
来源：http://zrg.nwbrower.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jgp.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://twy.wangshuangyany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ulo.shzxlz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uqs.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://hdf.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tqv.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ifc.tian-w.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cwx.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oce.gzhubu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xnw.haohaochexian.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wkz.zhoulong.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cmg.iojbl.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cmk.zdbjq.cn

[K07] 进制转换
来源：http://htc.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jru.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uzn.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dqp.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gjr.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://giq.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dzx.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mil.ydjk.org.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://csc.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://kkn.daria6918.cn

Py:   pickle.dumps(obj)
来源：http://tst.cdnleiting.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jrf.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://gmx.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://ynz.zhaomingkeji.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rht.gaohongyu789.top

Go:   encoding/gob
来源：http://bpv.guannengcc.top

Ruby: Marshal.dump(obj)
来源：http://rck.cqqwz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yua.ctjpmb.com

================================================================================
来源：http://qxu.yj202588.top

L. 网络请求
来源：http://hwd.cucudq.cn

================================================================================
来源：http://ymg.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://jrb.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kjz.redwolf501.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://enc.kuanghao11.cn

JS:   await fetch(url)
来源：http://idc.sweek.top

TS:   await fetch(url)
来源：http://brb.redwolf501.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jnq.yuxming.cn

Go:   resp, err := http.Get(url)
来源：http://quc.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lam.ydzc1.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mze.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://hyu.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jam.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ffs.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://quv.epnwcf.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wgb.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://twt.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xyf.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ekn.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lqv.haohaochexian.top

[L03] 设置自定义请求头
来源：http://wop.zhaomingkeji.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://urj.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uzj.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oxd.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dtd.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://boi.snrcjt.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xom.cucudq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://csc.cdnleiting.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xhq.hysaishi.cn

[L04] 设置超时
来源：http://nbo.iojbl.cn

Py:   requests.get(url, timeout=5)
来源：http://sbi.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vzr.hongshengwenyu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jqe.jinghuilouyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fpt.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://arn.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lkl.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ogy.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ofm.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://pfu.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wad.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tte.jinqigfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://prk.ywan-chungtsiang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lhn.gogol.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pzx.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xcj.ehwqpu.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dmt.ydzc1.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tja.yvedp.cn

[L06] 解析响应为 JSON
来源：http://oak.shzxlz.cn

Py:   resp.json()
来源：http://qgk.cashguo.top

PHP:  json_decode($body, true);
来源：http://err.sysykeji.top

JS:   await resp.json()
来源：http://cjv.cheryme.top

TS:   await resp.json()
来源：http://ffx.zhijiandao.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lnd.yongpay.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gbh.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://epm.dianchejie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uep.yuxming.cn

[L07] 处理 HTTP 状态码
来源：http://dlc.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ntp.ydzc1.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fwb.ivvv.top

JS:   resp.ok;  resp.status
来源：http://spi.hcnkem.com

TS:   resp.ok;  resp.status
来源：http://qgd.andypj.xyz

Java: resp.statusCode()
来源：http://vzc.hesvh.cn

Go:   resp.StatusCode
来源：http://nht.jinyuanbaomall.cn

Ruby: resp.code.to_i
来源：http://czj.yj20258888.top

C#:   (int)resp.StatusCode
来源：http://eon.shzxlz.cn

[L08] 并发请求多个地址
来源：http://qyq.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hhi.daxiang520.top

PHP:  curl_multi_init() 系列
来源：http://kdl.316326.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wma.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qfz.tanke756.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rdi.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eur.sweek.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xpb.bbcook.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wzb.0kj1m.cn

================================================================================
来源：http://mav.kuanghao11.cn

M. 命令行 / 进程 / 环境
来源：http://esp.nanxuanxn.top

================================================================================
来源：http://xaz.snrcjt.cn

[M01] 读取命令行参数
来源：http://mtj.zdbjq.cn

Py:   sys.argv[1:]
来源：http://lda.zhaomingkeji.xyz

PHP:  $argv;  $argc;
来源：http://rvt.pycfn.com

JS:   process.argv.slice(2)
来源：http://dhn.ivvv.top

TS:   process.argv.slice(2)
来源：http://joi.xinyue.icu

Java: args 数组（main 方法参数）
来源：http://rue.zhijiandao.cn

Go:   os.Args[1:]
来源：http://pvf.zhixingplan.top

Ruby: ARGV
来源：http://gai.daxiang520.top

C#:   args 数组（Main 方法参数）
来源：http://czf.jinqigufen.top

[M02] 读取环境变量
来源：http://uqf.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://prt.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ecb.ybcxt.top

JS:   process.env.HOME
来源：http://zlu.shanyushiyangkeji.top

TS:   process.env.HOME
来源：http://wai.xziqi.cn

Java: System.getenv("HOME")
来源：http://sza.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gjg.shuidangran.top

Ruby: ENV["HOME"]
来源：http://iyp.daxiang520.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qji.hesvh.cn

[M03] 执行外部命令
来源：http://jcv.hnqzz.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zmc.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wbm.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bsy.zhoulong.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://xwt.zdbjq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ptc.cashguo.top

Go:   exec.Command("ls", "-l").Output()
来源：http://aby.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://sdq.ydjk.org.cn

C#:   Process.Start("ls", "-l");
来源：http://odj.iojbl.cn

[M04] 获取当前工作目录
来源：http://ejr.birdmap.top

Py:   os.getcwd()
来源：http://ldf.shuidangran.top

PHP:  getcwd();
来源：http://aic.chenlongwang.top

JS:   process.cwd()
来源：http://lma.sufxvd.cn

TS:   process.cwd()
来源：http://djn.kuanghao11.cn

Java: Path.of("").toAbsolutePath()
来源：http://kmx.yangfankeji.com

Go:   os.Getwd()
来源：http://mcv.yuanzhike.top

Ruby: Dir.pwd
来源：http://wbo.xylfe.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ykw.xuanzx.com

[M05] 设置退出码
来源：http://hqj.yuxming.cn

Py:   sys.exit(1)
来源：http://cnd.ivvv.top

PHP:  exit(1);
来源：http://izs.jqgfzy.top

JS:   process.exit(1)
来源：http://vsb.jiagoushi.top

TS:   process.exit(1)
来源：http://xfl.ivvv.top

Java: System.exit(1)
来源：http://dbf.birdmap.top

Go:   os.Exit(1)
来源：http://qhk.jiagoushi.top

Ruby: exit 1
来源：http://bsa.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ztk.daria6918.cn

[M06] 向标准错误输出
来源：http://gqj.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://okm.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kts.snrcjt.cn

JS:   console.error("err")
来源：http://qwd.vqdsnc.cn

TS:   console.error("err")
来源：http://dfk.ydjk.org.cn

Java: System.err.println("err")
来源：http://vtu.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vhf.vehdjk.com

Ruby: warn "err"
来源：http://zuf.fengsongda.top

C#:   Console.Error.WriteLine("err")
来源：http://pvb.yuxming.cn

[M07] 判断是否为主入口
来源：http://mow.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://ifc.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rpc.feifeiyinyue.top

JS:   require.main === module
来源：http://csv.sysykeji.top

TS:   require.main === module
来源：http://vme.yueranfly.top

Java: public static void main(String[] args)
来源：http://oik.shanyushiyangkeji.top

Go:   func main()
来源：http://ukh.pengpengdd.cyou

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mow.yanxiufei.cn

C#:   static void Main(string[] args)
来源：http://bvz.smart0.xyz

[M08] 获取系统与运行时信息
来源：http://phv.epnwcf.com

Py:   platform.system();  platform.python_version()
来源：http://jkh.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://sdw.yj20258888.top

JS:   process.platform;  process.version
来源：http://dvc.cucudq.cn

TS:   process.platform;  process.version
来源：http://rmx.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nzd.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ada.snrcjt.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kct.yj20258.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nwc.yueranfly.top

================================================================================
来源：http://oyw.hnqzz.top

N. 数据结构与算法
来源：http://bir.jinqigufen.top

================================================================================
来源：http://imo.sxryk.cn

[N01] 二分查找（有序数组）
来源：http://nxn.52xcode.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kvt.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ali.bjfxy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://urc.cucudq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rxs.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qgf.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://rux.guannengcc.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dgv.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://sul.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://agh.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qxr.aizwys.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qxu.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vnp.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fyd.shangyingyoupin.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fix.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://ffp.ppjwa.cn

Ruby: arr.sort
来源：http://ulw.quarkkingdee.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jmq.quarkkingdee.top

[N03] 快速排序（分治示例）
来源：http://ygv.ehwqpu.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ckc.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://pbu.fehbvm.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qhw.ehwqpu.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qwf.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nwk.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hdg.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bcc.jiagoushi.top

C#:   // 手写递归，或 Array.Sort
来源：http://tuy.yongpay.top

[N04] 斐波那契数列
来源：http://ydh.zdqjudy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rdx.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wvt.meibo888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://spr.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bqb.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yse.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vov.vehdjk.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aki.fanxiaobao.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jxt.ydjk.org.cn

[N05] 最大公约数
来源：http://faz.zhijiandao.cn

Py:   math.gcd(a, b)
来源：http://cem.xuetiantiany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nrc.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gxf.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fyw.haohaochexian.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vxp.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eym.yj20258888.top

Ruby: a.gcd(b)
来源：http://ayv.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lzs.hnxiangtu.top

[N06] 判断回文字符串
来源：http://edc.cashguo.top

Py:   s == s[::-1]
来源：http://pwn.aizwys.cn

PHP:  $s === strrev($s);
来源：http://aif.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://ghm.epnwcf.com

TS:   s === [...s].reverse().join("")
来源：http://arf.sweek.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hfn.cashguo.top

Go:   // 双指针从两端比较
来源：http://fbr.gaohongyu789.top

Ruby: s == s.reverse
来源：http://vyd.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://aqb.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://tvt.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://moi.jyoumei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tuh.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://scf.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://dgq.andypj.xyz

Java: // 手写 HashMap
来源：http://ipg.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://pie.xziqi.cn

Ruby: // 手写 Hash
来源：http://pvr.yuanzhike.top

C#:   // 手写 Dictionary<int, int>
来源：http://pfu.shzxlz.cn

[N08] 生成全排列
来源：http://hwk.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://nup.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://kjz.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://stl.gogol.net.cn

TS:   // 手写回溯递归
来源：http://yds.9152youxi.cn

Java: // 手写回溯递归
来源：http://mmw.yj20258888.top

Go:   // 手写回溯递归
来源：http://kvb.dashuyun.cn

Ruby: arr.permutation.to_a
来源：http://tnh.hywenlv.cn

C#:   // 手写回溯递归
来源：http://lmx.ybcxt.top

[N09] 栈与队列
来源：http://pwp.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xbh.yvedp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://psf.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wrg.xuetiantiany.cn


<!-- 参考信息 -->