代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://dre.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mar.havefunace.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fwi.shanyushiyangtech.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xwc.xinyue.icu

Ruby: JSON.pretty_generate(obj)
来源：http://eab.nanxinkj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://evj.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://qtx.fzhhl.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://snr.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dmj.ybcxt.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jge.daria6918.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://grg.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bfp.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rnc.cqqwz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bjg.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zwk.hnxiangtu.top

[K05] 深拷贝对象
来源：http://adx.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://toy.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://shc.xylfe.cn

JS:   structuredClone(obj)
来源：http://tuw.yfazqb.com

TS:   structuredClone(obj)
来源：http://jjb.quarkkingdee.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dne.ydzc1.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ekr.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://amh.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zdw.fehbvm.com

[K06] 解析 URL 查询串
来源：http://dto.fehbvm.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uyb.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qtn.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xjv.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kym.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cjn.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://eue.epnwcf.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ybo.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tbj.feifeiyinyue.top

[K07] 进制转换
来源：http://tgo.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://luc.zhijiandao.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://raa.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cil.ehwqpu.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oqv.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xhg.yj20258888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lcd.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mwu.ehwqpu.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://djj.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://krf.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://qfg.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ivz.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://kpd.xuanzx.com

TS:   v8.serialize(obj)        // Node
来源：http://ppb.fehbvm.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nmw.shuidangran.top

Go:   encoding/gob
来源：http://acs.guowangkeji.top

Ruby: Marshal.dump(obj)
来源：http://xti.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uxo.vehdjk.com

================================================================================
来源：http://ocu.hnxiangtu.top

L. 网络请求
来源：http://iuc.zhixingplan.top

================================================================================
来源：http://jdo.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://jmt.hongshengwenyu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yps.tian-w.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://teg.redwolf501.top

JS:   await fetch(url)
来源：http://quc.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://bor.iojbl.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gxc.aizwys.cn

Go:   resp, err := http.Get(url)
来源：http://khx.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nwu.hfpthk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rai.sweek.top

[L02] 发送 POST JSON
来源：http://neu.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://bqh.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fdy.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eoq.zhijiandao.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zuc.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iyp.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rxe.havefunace.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ovt.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bee.yueranfly.top

[L03] 设置自定义请求头
来源：http://rsl.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vvx.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ttf.yangfankeji.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://net.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wyh.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ivb.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ztu.sweek.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tsw.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nlz.bbcook.cn

[L04] 设置超时
来源：http://fkl.jqgufenzy.top

Py:   requests.get(url, timeout=5)
来源：http://hkz.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zfb.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ntm.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oir.jqgfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nio.c1oappe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://swo.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rfo.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ztz.fanxiaobao.xyz

[L05] 上传文件（multipart）
来源：http://vwy.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tsm.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fgh.hammf.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xju.xuetiantiany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sqa.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qmp.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jkb.chenlongwang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pav.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vgk.ywan-chungtsiang.top

[L06] 解析响应为 JSON
来源：http://qwp.aizwys.cn

Py:   resp.json()
来源：http://gdl.zdqjudy.top

PHP:  json_decode($body, true);
来源：http://tvz.tianlin.xyz

JS:   await resp.json()
来源：http://kjw.52xcode.cn

TS:   await resp.json()
来源：http://gnr.redwolf501.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ssy.hywenlv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://elf.ctjpmb.com

Ruby: JSON.parse(resp.body)
来源：http://pvc.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wbk.cheryme.top

[L07] 处理 HTTP 状态码
来源：http://naa.yonumen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xlb.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://frz.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://bzb.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://fwx.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://jkw.hywenlv.cn

Go:   resp.StatusCode
来源：http://dit.tanke756.top

Ruby: resp.code.to_i
来源：http://hae.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://ugg.ybcxt.top

[L08] 并发请求多个地址
来源：http://jxb.havefunace.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qme.ehwqpu.com

PHP:  curl_multi_init() 系列
来源：http://enn.zhengqikj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qdl.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wlz.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ttm.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://foc.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://moy.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kaj.meibo888.top

================================================================================
来源：http://tff.haohaochexian.top

M. 命令行 / 进程 / 环境
来源：http://fld.uphjek.com

================================================================================
来源：http://dcc.hfpthk.cn

[M01] 读取命令行参数
来源：http://kul.tarul.cn

Py:   sys.argv[1:]
来源：http://muz.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://gam.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://wnt.xingfuxueyuan.xyz

TS:   process.argv.slice(2)
来源：http://iwl.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://wtm.chenzaomai.com

Go:   os.Args[1:]
来源：http://qgm.guannengcc.top

Ruby: ARGV
来源：http://wab.yfazqb.com

C#:   args 数组（Main 方法参数）
来源：http://dvh.ybcxt.top

[M02] 读取环境变量
来源：http://ylp.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://mnu.ydjk.org.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cuc.pengpengdd.cyou

JS:   process.env.HOME
来源：http://ahg.hfpthk.cn

TS:   process.env.HOME
来源：http://odb.ctjpmb.com

Java: System.getenv("HOME")
来源：http://hln.zhijiandao.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dmr.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://fxv.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pll.shangyingyoupin.top

[M03] 执行外部命令
来源：http://bgn.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://via.hnqzz.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hxl.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hgf.ppjwa.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vbw.hongshengwenyu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fce.fzhhl.top

Go:   exec.Command("ls", "-l").Output()
来源：http://apm.jiagoushi.top

Ruby: system("ls -l");  `ls -l`
来源：http://qpv.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://xgn.shanyushiyangkeji.top

[M04] 获取当前工作目录
来源：http://hdm.daxiang520.top

Py:   os.getcwd()
来源：http://vfp.nwbrower.top

PHP:  getcwd();
来源：http://qvs.chenjidiqi.icu

JS:   process.cwd()
来源：http://alb.yvedp.cn

TS:   process.cwd()
来源：http://gjc.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://fps.cqqwz.cn

Go:   os.Getwd()
来源：http://jpm.tian-w.cn

Ruby: Dir.pwd
来源：http://bkp.ydzc1.top

C#:   Directory.GetCurrentDirectory()
来源：http://hjk.tian-w.cn

[M05] 设置退出码
来源：http://twg.tianlin.xyz

Py:   sys.exit(1)
来源：http://gwb.tanke756.top

PHP:  exit(1);
来源：http://cvz.hongshengwenyu.top

JS:   process.exit(1)
来源：http://hrm.wangshuangyany.cn

TS:   process.exit(1)
来源：http://yth.0kj1m.cn

Java: System.exit(1)
来源：http://zon.svipenyu.cn

Go:   os.Exit(1)
来源：http://sid.jianghu66.top

Ruby: exit 1
来源：http://lri.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bpf.zhixingplan.top

[M06] 向标准错误输出
来源：http://efe.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://kiw.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ndg.jianghu66.top

JS:   console.error("err")
来源：http://rtb.daria6918.cn

TS:   console.error("err")
来源：http://ehx.yfazqb.com

Java: System.err.println("err")
来源：http://rkx.xingfuxueyuan.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://btq.zhixingplan.top

Ruby: warn "err"
来源：http://xfw.ppjwa.cn

C#:   Console.Error.WriteLine("err")
来源：http://avz.kuanghao11.cn

[M07] 判断是否为主入口
来源：http://eav.fzhhl.top

Py:   if __name__ == "__main__":
来源：http://drn.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ltv.aibaodan.cn

JS:   require.main === module
来源：http://anl.uphjek.com

TS:   require.main === module
来源：http://kzw.shangyingyoupin.top

Java: public static void main(String[] args)
来源：http://wps.xylfe.cn

Go:   func main()
来源：http://oyl.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gbd.yueranfly.top

C#:   static void Main(string[] args)
来源：http://awu.bbcook.cn

[M08] 获取系统与运行时信息
来源：http://ago.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://cwx.aizwys.cn

PHP:  PHP_OS;  phpversion();
来源：http://atr.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://dds.yj20258888.top

TS:   process.platform;  process.version
来源：http://zqu.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://deg.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pfj.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mso.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mso.xuanzx.com

================================================================================
来源：http://qch.hesvh.cn

N. 数据结构与算法
来源：http://qov.shuidangran.top

================================================================================
来源：http://kvl.sweek.top

[N01] 二分查找（有序数组）
来源：http://zdn.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://gsb.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kpc.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bfb.sufxvd.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://syo.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://tsr.hammf.cn

Go:   sort.SearchInts(arr, x)
来源：http://moy.andypj.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://egc.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://kzw.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://gcr.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://ijm.yvedp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xba.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ufj.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://auv.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wob.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://fbb.meibo888.top

Ruby: arr.sort
来源：http://qxq.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mhb.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://bxs.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qhb.cucudq.cn

PHP:  // 递归实现，或用 usort
来源：http://xvs.zhongyouzk.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aja.316326.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qwo.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://umo.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pkw.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qqq.yangfankeji.com

C#:   // 手写递归，或 Array.Sort
来源：http://erh.redwolf501.top

[N04] 斐波那契数列
来源：http://hjp.hywenlv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rqk.xuetiantiany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xog.yonumen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ydk.gotoacloud.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ibz.zhiwuduotai.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://spp.xylfe.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tqm.yuanzhike.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zxc.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jgp.smart0.xyz

[N05] 最大公约数
来源：http://aun.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://ybp.xuanzx.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dsr.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qel.guowangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dre.shanyushiyangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://crk.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pan.yanxiufei.cn

Ruby: a.gcd(b)
来源：http://zek.uphjek.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ynv.gotoacloud.top

[N06] 判断回文字符串
来源：http://ovg.nanxinkj.top

Py:   s == s[::-1]
来源：http://gzm.cashguo.top

PHP:  $s === strrev($s);
来源：http://mgp.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://edf.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://hwe.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kqi.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://ngo.hysaishi.cn

Ruby: s == s.reverse
来源：http://rrf.tanke756.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xpu.ywan-chungtsiang.top

[N07] 两数之和（返回下标）
来源：http://dnh.zhixingplan.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uvv.sufxvd.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://exc.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dxu.fktsv.cn

TS:   // 手写 Map<string, number>
来源：http://fkk.shangyingyoupin.top

Java: // 手写 HashMap
来源：http://wxz.xinyue.icu

Go:   // 手写 map[int]int
来源：http://ene.yvedp.cn

Ruby: // 手写 Hash
来源：http://ocm.zhiwuduotai.top

C#:   // 手写 Dictionary<int, int>
来源：http://vha.gaohongyu789.top

[N08] 生成全排列
来源：http://wzq.ybcxt.top

Py:   itertools.permutations(arr)
来源：http://djf.jlsjyb.cn

PHP:  // 手写递归交换
来源：http://pyt.shuidangran.top

JS:   // 手写回溯递归
来源：http://brp.zhengqikj.top

TS:   // 手写回溯递归
来源：http://egk.bbcook.cn

Java: // 手写回溯递归
来源：http://jkp.redwolf501.top

Go:   // 手写回溯递归
来源：http://lnz.zhoulong.xyz

Ruby: arr.permutation.to_a
来源：http://xme.redwolf501.top

C#:   // 手写回溯递归
来源：http://lev.yangfankeji.com

[N09] 栈与队列
来源：http://wve.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vws.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fqn.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jcn.fehbvm.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pga.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wjg.zdbjq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ayl.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bfi.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cao.hnqzz.top

[N10] 链表节点定义
来源：http://ocy.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://umb.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hhp.jiagoushi.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sxt.zhijiandao.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vhl.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://zvr.xziqi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sww.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://aqj.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mxi.316326.xyz

[N11] 二叉树中序遍历
来源：http://xgc.jqgfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://myz.pycfn.com

PHP:  // 手写递归函数
来源：http://jen.yvedp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rgy.hammf.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lco.sysykeji.top

Java: // 手写递归
来源：http://qai.shuidangran.top


<!-- 参考信息 -->