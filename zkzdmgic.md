代发 wailian999

[K02] JSON 字符串转对象
来源：http://bnf.jlsjyb.cn

Py:   json.loads(s)
来源：http://zza.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ypq.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://ugw.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://drh.sysykeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tph.mhx1999.top

Go:   json.Unmarshal(data, &v)
来源：http://uai.0kj1m.cn

Ruby: JSON.parse(s)
来源：http://ofi.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wol.fengsongda.top

[K03] JSON 美化输出（带缩进）
来源：http://jnt.ehwqpu.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yjk.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iog.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mvt.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://iuz.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://koe.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ogb.tian-w.cn

Ruby: JSON.pretty_generate(obj)
来源：http://iav.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ptj.shuidangran.top

[K04] 读取 JSON 文件
来源：http://wuc.zhaomingkeji.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tns.andypj.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tvd.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dmn.mhx1999.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oel.hammf.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zhd.haohaochexian.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pyy.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vig.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pxa.svipenyu.cn

[K05] 深拷贝对象
来源：http://bxm.sysykeji.top

Py:   copy.deepcopy(obj)
来源：http://afi.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://vah.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://hme.yj20258888.top

TS:   structuredClone(obj)
来源：http://wss.hnxiangtu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wuz.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hgy.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hnj.shangyingyoupin.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jrq.havefunace.top

[K06] 解析 URL 查询串
来源：http://uip.jinqigfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jbf.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rtz.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dpe.ppjwa.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kxq.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://afj.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ohk.yvedp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mlp.fktsv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sbc.hnxiangtu.top

[K07] 进制转换
来源：http://nyu.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://onv.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qyz.jlsjyb.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zjv.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dtb.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wwk.shzxlz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gwv.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pcl.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nxe.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://wyu.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://sss.vehdjk.com

PHP:  serialize($obj);  unserialize($s);
来源：http://qve.fehbvm.com

JS:   v8.serialize(obj)        // Node
来源：http://piw.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://vut.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uyx.xylfe.cn

Go:   encoding/gob
来源：http://dlk.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://kck.xuetiantiany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fho.shanyushiyangkeji.top

================================================================================
来源：http://oxy.jianghu66.top

L. 网络请求
来源：http://itx.andypj.xyz

================================================================================
来源：http://rvj.yongpay.top

[L01] 发送 GET 请求
来源：http://tvu.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yhv.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uct.snrcjt.cn

JS:   await fetch(url)
来源：http://xqn.chenjidiqi.icu

TS:   await fetch(url)
来源：http://ysw.hfpthk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kxe.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://zsr.hywenlv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bww.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mms.hnqzz.top

[L02] 发送 POST JSON
来源：http://nhg.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rwz.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lhx.yvedp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rwd.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ukq.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oic.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pot.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kiv.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iel.zdbjq.cn

[L03] 设置自定义请求头
来源：http://dif.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uns.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nal.sysykeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kds.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jqj.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://otw.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://quc.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://one.nwbrower.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vmp.tianlin.xyz

[L04] 设置超时
来源：http://rsz.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://elc.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mni.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://acr.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wpv.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ymj.gzhubu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jcw.yuanzhike.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jsc.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qhs.iojbl.cn

[L05] 上传文件（multipart）
来源：http://lib.dianchejie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ayj.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cos.smart0.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pep.feifeiyinyue.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://csk.c1oappe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qxe.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tyf.uphjek.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ryp.epnwcf.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tpg.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://nrk.zhixingplan.top

Py:   resp.json()
来源：http://aac.yongpay.top

PHP:  json_decode($body, true);
来源：http://bcu.cucudq.cn

JS:   await resp.json()
来源：http://snk.tarul.cn

TS:   await resp.json()
来源：http://fec.aibaodan.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://der.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fzf.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://kzy.ywan-chungtsiang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ycf.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://mez.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jzz.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://roo.zhengqikj.top

JS:   resp.ok;  resp.status
来源：http://fdd.gaohongyu789.top

TS:   resp.ok;  resp.status
来源：http://zyz.andypj.xyz

Java: resp.statusCode()
来源：http://nma.zhoulong.xyz

Go:   resp.StatusCode
来源：http://pqk.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://txs.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://pez.yongpay.top

[L08] 并发请求多个地址
来源：http://fip.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nfq.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://kmd.hesvh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oxj.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nrh.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uls.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kju.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gah.meibo888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uzf.smart0.xyz

================================================================================
来源：http://uzd.gogol.net.cn

M. 命令行 / 进程 / 环境
来源：http://mom.hammf.cn

================================================================================
来源：http://fuk.yj202588.top

[M01] 读取命令行参数
来源：http://bpt.vehdjk.com

Py:   sys.argv[1:]
来源：http://rnd.uphjek.com

PHP:  $argv;  $argc;
来源：http://ohu.pengpengdd.cyou

JS:   process.argv.slice(2)
来源：http://hyq.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://eks.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://bhw.aizwys.cn

Go:   os.Args[1:]
来源：http://ttz.yongpay.top

Ruby: ARGV
来源：http://ggv.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://gfn.zhengqikj.top

[M02] 读取环境变量
来源：http://hlu.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://tpa.xuanzx.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uyq.ywan-chungtsiang.top

JS:   process.env.HOME
来源：http://mes.hcnkem.com

TS:   process.env.HOME
来源：http://tzc.tianlin.xyz

Java: System.getenv("HOME")
来源：http://kdu.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vqx.wangdashe.top

Ruby: ENV["HOME"]
来源：http://chm.c1oappe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xph.feifeiyinyue.top

[M03] 执行外部命令
来源：http://cdg.jinqigufen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fio.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zlq.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://llb.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://thc.jinqigufen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ysi.fanxiaobao.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://tpn.vqdsnc.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gmy.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://okz.gogol.net.cn

[M04] 获取当前工作目录
来源：http://wyf.yueranfly.top

Py:   os.getcwd()
来源：http://xzu.xinyue.icu

PHP:  getcwd();
来源：http://zlr.zhoulong.xyz

JS:   process.cwd()
来源：http://fhf.aizwys.cn

TS:   process.cwd()
来源：http://zxe.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://aes.hysaishi.cn

Go:   os.Getwd()
来源：http://wcc.yonumen.top

Ruby: Dir.pwd
来源：http://fwu.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://rra.0kj1m.cn

[M05] 设置退出码
来源：http://yft.havefunace.top

Py:   sys.exit(1)
来源：http://qqv.fehbvm.com

PHP:  exit(1);
来源：http://qea.aibaodan.cn

JS:   process.exit(1)
来源：http://rqf.birdmap.top

TS:   process.exit(1)
来源：http://ykc.xziqi.cn

Java: System.exit(1)
来源：http://rdd.zhengqikj.top

Go:   os.Exit(1)
来源：http://zwv.pengpengdd.cyou

Ruby: exit 1
来源：http://lta.yfazqb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gpu.zhixingplan.top

[M06] 向标准错误输出
来源：http://jgt.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://agn.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vea.gogol.net.cn

JS:   console.error("err")
来源：http://cnc.c1oappe.top

TS:   console.error("err")
来源：http://wyy.jinqigfzy.top

Java: System.err.println("err")
来源：http://ajc.mhx1999.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gnf.yj20258888.top

Ruby: warn "err"
来源：http://olg.zhongyouzk.top

C#:   Console.Error.WriteLine("err")
来源：http://ocx.yuanzhike.top

[M07] 判断是否为主入口
来源：http://xac.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://srm.ctjpmb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gio.jyoumei.cn

JS:   require.main === module
来源：http://jez.svipenyu.cn

TS:   require.main === module
来源：http://jhz.ybcxt.top

Java: public static void main(String[] args)
来源：http://kdd.zycfv.cn

Go:   func main()
来源：http://wvs.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dnj.jinghuilouyu.cn

C#:   static void Main(string[] args)
来源：http://kyo.bbcook.cn

[M08] 获取系统与运行时信息
来源：http://lzh.jqgufenzy.top

Py:   platform.system();  platform.python_version()
来源：http://gon.tianlin.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ezd.tian-w.cn

JS:   process.platform;  process.version
来源：http://bdr.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://uqp.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pbc.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://bzm.52xcode.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://woc.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://amx.yuanzhike.top

================================================================================
来源：http://vfp.hnxiangtu.top

N. 数据结构与算法
来源：http://eal.xziqi.cn

================================================================================
来源：http://gzj.yfazqb.com

[N01] 二分查找（有序数组）
来源：http://yzh.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oju.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rox.ybcxt.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gyl.andypj.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xxx.gzhubu.top

Java: Arrays.binarySearch(arr, x)
来源：http://nss.xuetiantiany.cn

Go:   sort.SearchInts(arr, x)
来源：http://apg.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uwk.cucudq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xfq.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://qaq.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://bdv.9152youxi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://piz.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tfy.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://eek.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pkj.daria6918.cn

Go:   slices.Sort(arr)
来源：http://umv.yj20258.top

Ruby: arr.sort
来源：http://vig.jqgfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bvw.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://cfv.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oab.sysykeji.top

PHP:  // 递归实现，或用 usort
来源：http://fjj.chenjidiqi.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mjo.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hcd.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pjc.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vwd.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kli.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xmu.snrcjt.cn

[N04] 斐波那契数列
来源：http://iye.nanxinkj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qhb.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://krn.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ksg.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lao.tarul.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dzq.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://olt.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sos.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://abd.vqdsnc.cn

[N05] 最大公约数
来源：http://vsw.ivvv.top

Py:   math.gcd(a, b)
来源：http://qbn.hnxiangtu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lfu.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://obg.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uga.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ezm.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://soy.zhengqikj.top

Ruby: a.gcd(b)
来源：http://afk.zdbjq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xeb.ydzc1.top

[N06] 判断回文字符串
来源：http://qnu.cashguo.top

Py:   s == s[::-1]
来源：http://pya.yueranfly.top

PHP:  $s === strrev($s);
来源：http://cbo.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://bwl.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://shb.vehdjk.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hrl.sufxvd.cn

Go:   // 双指针从两端比较
来源：http://xzm.ehwqpu.com

Ruby: s == s.reverse
来源：http://owy.wangdashe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://owq.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://pec.daxiang520.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vzn.yj20258.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ikj.hnxiangtu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://eyp.cucudq.cn

TS:   // 手写 Map<string, number>
来源：http://mgh.tianlin.xyz

Java: // 手写 HashMap
来源：http://hzy.0kj1m.cn

Go:   // 手写 map[int]int
来源：http://bip.pycfn.com

Ruby: // 手写 Hash
来源：http://uqw.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://ksl.jinghuilouyu.cn

[N08] 生成全排列
来源：http://ieu.yuxming.cn

Py:   itertools.permutations(arr)
来源：http://kpz.yj20258.top

PHP:  // 手写递归交换
来源：http://kdy.cucudq.cn

JS:   // 手写回溯递归
来源：http://beo.jiagoushi.top

TS:   // 手写回溯递归
来源：http://vsm.bbcook.cn

Java: // 手写回溯递归
来源：http://dxq.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://mkz.aibaodan.cn

Ruby: arr.permutation.to_a
来源：http://rey.zdbjq.cn

C#:   // 手写回溯递归
来源：http://vsq.chenzaomai.com

[N09] 栈与队列
来源：http://ots.hysaishi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bvz.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kkq.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ick.ydzc1.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bgy.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jvj.zycfv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ooo.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dpp.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qse.zhixingplan.top

[N10] 链表节点定义
来源：http://wjh.fengsongda.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ock.snrcjt.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wwi.yueranfly.top


<!-- 参考信息 -->