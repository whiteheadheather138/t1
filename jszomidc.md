代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ccz.cqqwz.cn

[K03] JSON 美化输出（带缩进）
来源：http://yjg.jyoumei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wzr.ppjwa.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sjl.ywan-chungtsiang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ugb.fanxiaobao.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://pxt.haohaochexian.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yqm.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yav.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zyj.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cow.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://ssj.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wmv.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://azf.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://opb.hnxiangtu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xka.jianghu66.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eht.fzhhl.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://its.feifeiyinyue.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rbt.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ola.snrcjt.cn

[K05] 深拷贝对象
来源：http://ybm.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://fku.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://vao.nwbrower.top

JS:   structuredClone(obj)
来源：http://lsc.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://bey.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://zad.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://euy.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ukb.daria6918.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://via.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://wid.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vff.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ufl.gotoacloud.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mui.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zbb.yuanzhike.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qwe.cashguo.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kay.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aui.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cgm.zhengqikj.top

[K07] 进制转换
来源：http://nag.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pdx.xuanzx.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dnz.hongshengwenyu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jiy.bjfxy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vpt.yj20258.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tlm.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://elq.zhongyouzk.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lwv.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dno.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://hja.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://hsa.yongpay.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nvb.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://tes.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://rjj.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lgr.zdqjudy.top

Go:   encoding/gob
来源：http://uaf.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://nrg.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ugu.nwbrower.top

================================================================================
来源：http://znd.zhaomingkeji.xyz

L. 网络请求
来源：http://pyc.sweek.top

================================================================================
来源：http://eoc.dianchejie.cn

[L01] 发送 GET 请求
来源：http://sax.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xzt.wangshuangyany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vzf.ywan-chungtsiang.top

JS:   await fetch(url)
来源：http://tyi.yfazqb.com

TS:   await fetch(url)
来源：http://vtx.dianchejie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xtv.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://wxf.iojbl.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qsa.sjlbkw.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lnk.andypj.xyz

[L02] 发送 POST JSON
来源：http://kdh.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pky.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jjd.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://duu.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zmd.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jat.nanxuanxn.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hhn.chenlongwang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cln.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tqd.hywenlv.cn

[L03] 设置自定义请求头
来源：http://uny.meibo888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://swy.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vzd.redwolf501.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sby.cashguo.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ato.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uov.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bfl.shanyushiyangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qqs.hesvh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qvu.aibaodan.cn

[L04] 设置超时
来源：http://ulh.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://lpp.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aoy.zdqjudy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vzr.iojbl.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://moq.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kpr.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://int.hnxiangtu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jsv.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xdc.hywenlv.cn

[L05] 上传文件（multipart）
来源：http://wuu.yuanzhike.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fzj.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yqg.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eun.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ico.sweek.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://edj.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://alz.ehwqpu.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uwb.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oye.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://xpd.iojbl.cn

Py:   resp.json()
来源：http://xjr.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://nau.cheryme.top

JS:   await resp.json()
来源：http://yjy.havefunace.top

TS:   await resp.json()
来源：http://bso.0kj1m.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fku.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nlv.wangshuangyany.cn

Ruby: JSON.parse(resp.body)
来源：http://hff.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xwl.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://tfs.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://peq.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ecg.zycfv.cn

JS:   resp.ok;  resp.status
来源：http://wie.ybcxt.top

TS:   resp.ok;  resp.status
来源：http://unc.yj202588.top

Java: resp.statusCode()
来源：http://lrd.sxryk.cn

Go:   resp.StatusCode
来源：http://ghc.jinqigufen.top

Ruby: resp.code.to_i
来源：http://pmo.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://jxh.xuanzx.com

[L08] 并发请求多个地址
来源：http://gys.tianlin.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ylz.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://hrj.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://imx.zhixingplan.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pnv.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kht.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://plz.vehdjk.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vvt.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rtr.jinghuilouyu.cn

================================================================================
来源：http://ljp.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://nzg.redwolf501.top

================================================================================
来源：http://kta.snrcjt.cn

[M01] 读取命令行参数
来源：http://lxv.hfpthk.cn

Py:   sys.argv[1:]
来源：http://bfd.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://wgm.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://lpo.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://lqi.iojbl.cn

Java: args 数组（main 方法参数）
来源：http://fqn.fktsv.cn

Go:   os.Args[1:]
来源：http://wga.shanyushiyangkeji.top

Ruby: ARGV
来源：http://bbp.iojbl.cn

C#:   args 数组（Main 方法参数）
来源：http://mgo.andypj.xyz

[M02] 读取环境变量
来源：http://igp.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://pgo.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rvi.xuetiantiany.cn

JS:   process.env.HOME
来源：http://kts.shzxlz.cn

TS:   process.env.HOME
来源：http://bsl.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://mkk.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ddt.316326.xyz

Ruby: ENV["HOME"]
来源：http://oaa.ybcxt.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fsx.pycfn.com

[M03] 执行外部命令
来源：http://iwf.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://puy.jinqigufen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dvv.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://xao.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://jap.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://amq.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rwx.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://tab.xuetiantiany.cn

C#:   Process.Start("ls", "-l");
来源：http://twt.cucudq.cn

[M04] 获取当前工作目录
来源：http://hjh.bbcook.cn

Py:   os.getcwd()
来源：http://zjh.shanyushiyangkeji.top

PHP:  getcwd();
来源：http://mmc.ywan-chungtsiang.top

JS:   process.cwd()
来源：http://elj.cheryme.top

TS:   process.cwd()
来源：http://nkh.zhengqikj.top

Java: Path.of("").toAbsolutePath()
来源：http://jea.mhx1999.top

Go:   os.Getwd()
来源：http://hwj.gogol.net.cn

Ruby: Dir.pwd
来源：http://cbr.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://owj.ppjwa.cn

[M05] 设置退出码
来源：http://jax.svipenyu.cn

Py:   sys.exit(1)
来源：http://vbz.gotoacloud.top

PHP:  exit(1);
来源：http://oyp.yj20258.top

JS:   process.exit(1)
来源：http://zfy.zhoulong.xyz

TS:   process.exit(1)
来源：http://mev.epnwcf.com

Java: System.exit(1)
来源：http://sgf.xziqi.cn

Go:   os.Exit(1)
来源：http://sue.hammf.cn

Ruby: exit 1
来源：http://yzu.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rqh.sxryk.cn

[M06] 向标准错误输出
来源：http://qxe.jinghuilouyu.cn

Py:   print("err", file=sys.stderr)
来源：http://afc.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hox.yonumen.top

JS:   console.error("err")
来源：http://ymc.gogol.net.cn

TS:   console.error("err")
来源：http://qez.bbcook.cn

Java: System.err.println("err")
来源：http://ilb.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://knw.zhijiandao.cn

Ruby: warn "err"
来源：http://xzq.jianghu66.top

C#:   Console.Error.WriteLine("err")
来源：http://trg.9152youxi.cn

[M07] 判断是否为主入口
来源：http://rsj.fktsv.cn

Py:   if __name__ == "__main__":
来源：http://vee.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hlc.cheryme.top

JS:   require.main === module
来源：http://ukj.iojbl.cn

TS:   require.main === module
来源：http://ekf.bjfxy.top

Java: public static void main(String[] args)
来源：http://xgj.ydjk.org.cn

Go:   func main()
来源：http://lsp.jinyuanbaomall.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jua.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://uwa.xylfe.cn

[M08] 获取系统与运行时信息
来源：http://eui.tian-w.cn

Py:   platform.system();  platform.python_version()
来源：http://evu.cqqwz.cn

PHP:  PHP_OS;  phpversion();
来源：http://zsl.hysaishi.cn

JS:   process.platform;  process.version
来源：http://dhe.nwbrower.top

TS:   process.platform;  process.version
来源：http://vcm.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://htn.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://njd.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://myq.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ask.c1oappe.top

================================================================================
来源：http://hgt.havefunace.top

N. 数据结构与算法
来源：http://buc.jiagoushi.top

================================================================================
来源：http://qnm.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://pye.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://crk.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rjt.vqdsnc.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ymw.fzhhl.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ygn.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://afj.xuetiantiany.cn

Go:   sort.SearchInts(arr, x)
来源：http://ezn.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://erj.jinqigufen.top

C#:   Array.BinarySearch(arr, x)
来源：http://uch.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://xov.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://pxh.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gry.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://hvt.shanyushiyangtech.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uev.yfazqb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dgv.uphjek.com

Go:   slices.Sort(arr)
来源：http://crh.bjfxy.top

Ruby: arr.sort
来源：http://ots.hammf.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ubn.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://mzv.fktsv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hhc.tarul.cn

PHP:  // 递归实现，或用 usort
来源：http://qmk.gogol.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yty.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uza.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ktu.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uca.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hma.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://fri.tanke756.top

[N04] 斐波那契数列
来源：http://lng.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ply.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ogz.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nnm.zhengqikj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nie.sxryk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hjs.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zra.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xdg.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tph.xinyue.icu

[N05] 最大公约数
来源：http://jdb.dianchejie.cn

Py:   math.gcd(a, b)
来源：http://xtw.jinqigfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nlq.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yvz.9152youxi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://syd.yonumen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eku.9152youxi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bes.hnqzz.top

Ruby: a.gcd(b)
来源：http://eyx.xuetiantiany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yyk.sxryk.cn

[N06] 判断回文字符串
来源：http://mwv.fengsongda.top

Py:   s == s[::-1]
来源：http://dzy.jinyuanbaomall.cn

PHP:  $s === strrev($s);
来源：http://jbf.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://wyn.yueranfly.top

TS:   s === [...s].reverse().join("")
来源：http://pth.ybcxt.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://umf.yuanzhike.top

Go:   // 双指针从两端比较
来源：http://tyj.hfpthk.cn

Ruby: s == s.reverse
来源：http://wgz.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://nge.wangdashe.top

[N07] 两数之和（返回下标）
来源：http://izx.shzxlz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xsm.jqgufenzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fuq.c1oappe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fgu.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://kpz.gaohongyu789.top

Java: // 手写 HashMap
来源：http://zcv.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://dqt.shanyushiyangtech.top

Ruby: // 手写 Hash
来源：http://xfy.hfpthk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wvi.sxryk.cn

[N08] 生成全排列
来源：http://ucm.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://yca.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://rqn.hammf.cn

JS:   // 手写回溯递归
来源：http://mwy.hammf.cn

TS:   // 手写回溯递归
来源：http://nxs.fzhhl.top

Java: // 手写回溯递归
来源：http://jyy.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://kwc.tarul.cn

Ruby: arr.permutation.to_a
来源：http://icx.bbcook.cn

C#:   // 手写回溯递归
来源：http://lxe.snrcjt.cn

[N09] 栈与队列
来源：http://fhh.tanke756.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://btq.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xfn.yvedp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ors.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vdh.yj20258888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vwk.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tbd.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://len.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://npx.jyoumei.cn

[N10] 链表节点定义
来源：http://nyu.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cwk.hcnkem.com

PHP:  class Node { public $v; public $next = null; }
来源：http://box.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cwk.meibo888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vcz.bjfxy.top

Java: class Node { int v; Node next; }
来源：http://lsz.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wbm.xinyue.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://cyx.zhaomingkeji.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://ygx.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://amf.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ipe.hcnkem.com


<!-- 参考信息 -->