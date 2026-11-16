代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://erl.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://wrc.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lsv.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tiy.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lxa.hammf.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gsc.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://umw.52xcode.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yuu.ctjpmb.com

Ruby: JSON.pretty_generate(obj)
来源：http://rjw.daria6918.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yki.zdbjq.cn

[K04] 读取 JSON 文件
来源：http://age.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ohv.havefunace.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sqf.jinghuilouyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wjw.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hoq.birdmap.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zzd.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ynz.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ugp.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dis.cucudq.cn

[K05] 深拷贝对象
来源：http://ifx.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://tci.andypj.xyz

PHP:  unserialize(serialize($obj));
来源：http://tww.tarul.cn

JS:   structuredClone(obj)
来源：http://hsv.bbcook.cn

TS:   structuredClone(obj)
来源：http://bqr.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kco.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qbk.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rdy.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jgr.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://dwa.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vln.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zjk.nanxinkj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ciw.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vzf.meibo888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cag.svipenyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ukl.yuanzhike.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pin.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://upf.xuanzx.com

[K07] 进制转换
来源：http://snx.jqgfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://edv.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hyr.epnwcf.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xjo.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://abo.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jcl.daria6918.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oqr.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uuv.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bfn.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://leb.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://zpp.shzxlz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kmb.svipenyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://vxj.ivvv.top

TS:   v8.serialize(obj)        // Node
来源：http://tmb.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://miv.wangshuangyany.cn

Go:   encoding/gob
来源：http://xyo.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://zmj.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zhx.zhengqikj.top

================================================================================
来源：http://jqi.snrcjt.cn

L. 网络请求
来源：http://eut.quarkkingdee.top

================================================================================
来源：http://njq.52xcode.cn

[L01] 发送 GET 请求
来源：http://sne.sufxvd.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zcn.fktsv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kok.gaohongyu789.top

JS:   await fetch(url)
来源：http://nsu.gzhubu.top

TS:   await fetch(url)
来源：http://ccp.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cwt.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://sox.jinghuilouyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jyk.fktsv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://waj.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://ekj.zdqjudy.top

Py:   requests.post(url, json={"a": 1})
来源：http://ywf.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ymw.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blh.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yir.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ifl.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gto.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ejc.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wes.aizwys.cn

[L03] 设置自定义请求头
来源：http://ohx.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://irv.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://epo.yanxiufei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mla.zhongyouzk.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lvp.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iic.snrcjt.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ver.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://itz.bbcook.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jhl.hcnkem.com

[L04] 设置超时
来源：http://jgk.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://eyz.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qva.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fna.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hzg.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yvn.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kmv.yongpay.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yax.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xps.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://qwp.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xuq.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wfi.xuanzx.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rra.yangfankeji.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yyu.chenlongwang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zuj.zycfv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zte.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gbt.mhx1999.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tfg.xinyue.icu

[L06] 解析响应为 JSON
来源：http://kyx.hnqzz.top

Py:   resp.json()
来源：http://igy.quarkkingdee.top

PHP:  json_decode($body, true);
来源：http://crj.zdbjq.cn

JS:   await resp.json()
来源：http://ugz.9152youxi.cn

TS:   await resp.json()
来源：http://pdn.316326.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qji.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zaq.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://kco.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mtg.snrcjt.cn

[L07] 处理 HTTP 状态码
来源：http://pjx.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tge.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qgo.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://ddu.cqqwz.cn

TS:   resp.ok;  resp.status
来源：http://uwl.yfazqb.com

Java: resp.statusCode()
来源：http://pib.xinyue.icu

Go:   resp.StatusCode
来源：http://zfz.fzhhl.top

Ruby: resp.code.to_i
来源：http://nwr.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://ofw.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://ztg.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zvk.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://ogy.yj20258.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lzo.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qji.hysaishi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://why.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bpp.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ssb.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bko.tarul.cn

================================================================================
来源：http://tdh.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://pqa.gogol.net.cn

================================================================================
来源：http://fec.redwolf501.top

[M01] 读取命令行参数
来源：http://avh.dianchejie.cn

Py:   sys.argv[1:]
来源：http://crz.yonumen.top

PHP:  $argv;  $argc;
来源：http://qjj.iojbl.cn

JS:   process.argv.slice(2)
来源：http://dmm.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://mvc.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://iry.cdnleiting.top

Go:   os.Args[1:]
来源：http://qxr.svipenyu.cn

Ruby: ARGV
来源：http://ldn.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://dqo.sxryk.cn

[M02] 读取环境变量
来源：http://vhs.zhixingplan.top

Py:   os.environ.get("HOME")
来源：http://fzm.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cka.cucudq.cn

JS:   process.env.HOME
来源：http://bjx.sjlbkw.cn

TS:   process.env.HOME
来源：http://gjc.jianghu66.top

Java: System.getenv("HOME")
来源：http://rnk.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dpn.hammf.cn

Ruby: ENV["HOME"]
来源：http://yap.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jbd.vqdsnc.cn

[M03] 执行外部命令
来源：http://ezv.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ofs.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lhc.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://aad.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wuq.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kms.ctjpmb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ddj.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uqa.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://xzo.zhijiandao.cn

[M04] 获取当前工作目录
来源：http://guc.vehdjk.com

Py:   os.getcwd()
来源：http://viw.vehdjk.com

PHP:  getcwd();
来源：http://uzz.xinyue.icu

JS:   process.cwd()
来源：http://trw.xuetiantiany.cn

TS:   process.cwd()
来源：http://dtu.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://pmk.dashuyun.cn

Go:   os.Getwd()
来源：http://ogn.zhixingplan.top

Ruby: Dir.pwd
来源：http://nux.bjfxy.top

C#:   Directory.GetCurrentDirectory()
来源：http://cze.hongshengwenyu.top

[M05] 设置退出码
来源：http://xju.sweek.top

Py:   sys.exit(1)
来源：http://lwu.svipenyu.cn

PHP:  exit(1);
来源：http://pcw.yj202588.top

JS:   process.exit(1)
来源：http://nat.jinghuilouyu.cn

TS:   process.exit(1)
来源：http://zou.ydjk.org.cn

Java: System.exit(1)
来源：http://skx.iojbl.cn

Go:   os.Exit(1)
来源：http://syi.jlsjyb.cn

Ruby: exit 1
来源：http://scc.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pbm.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://hyo.wangdashe.top

Py:   print("err", file=sys.stderr)
来源：http://dic.yj202588.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eip.dashuyun.cn

JS:   console.error("err")
来源：http://imo.svipenyu.cn

TS:   console.error("err")
来源：http://sdg.jlsjyb.cn

Java: System.err.println("err")
来源：http://ley.sjlbkw.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ixn.ctjpmb.com

Ruby: warn "err"
来源：http://ylo.xziqi.cn

C#:   Console.Error.WriteLine("err")
来源：http://sfn.yvedp.cn

[M07] 判断是否为主入口
来源：http://wqa.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://xim.gzhubu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jym.birdmap.top

JS:   require.main === module
来源：http://czb.jinqigufen.top

TS:   require.main === module
来源：http://tyq.hnqzz.top

Java: public static void main(String[] args)
来源：http://hmq.zhengqikj.top

Go:   func main()
来源：http://hdf.cheryme.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rqy.fehbvm.com

C#:   static void Main(string[] args)
来源：http://pmz.hnxiangtu.top

[M08] 获取系统与运行时信息
来源：http://zzn.xziqi.cn

Py:   platform.system();  platform.python_version()
来源：http://rxa.cucudq.cn

PHP:  PHP_OS;  phpversion();
来源：http://njc.cucudq.cn

JS:   process.platform;  process.version
来源：http://vvv.chenzaomai.com

TS:   process.platform;  process.version
来源：http://cdb.yonumen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jfi.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://bvj.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mgu.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tsj.jyoumei.cn

================================================================================
来源：http://ybn.guannengcc.top

N. 数据结构与算法
来源：http://ydy.cashguo.top

================================================================================
来源：http://hff.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://zdy.xylfe.cn

Py:   bisect.bisect_left(arr, x)
来源：http://imk.yj20258.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tye.yfazqb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dwt.gzhubu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lax.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://any.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://klr.gotoacloud.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://upi.jinghuilouyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zzm.guannengcc.top

[N02] 排序（工程实践用内置实现）
来源：http://hrm.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://uao.kuanghao11.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xgs.shanyushiyangtech.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pve.yuxming.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qab.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xan.hcnkem.com

Go:   slices.Sort(arr)
来源：http://abi.yanxiufei.cn

Ruby: arr.sort
来源：http://sqy.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://prv.shzxlz.cn

[N03] 快速排序（分治示例）
来源：http://nuh.shanyushiyangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nql.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://itt.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ass.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wsn.yvedp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tvh.wangdashe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hhw.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ahl.shzxlz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bxn.daxiang520.top

[N04] 斐波那契数列
来源：http://zqa.gzhubu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bli.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ldu.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://apb.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ndg.yvedp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yrf.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://soh.yuanzhike.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xpd.9152youxi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pnz.ehwqpu.com

[N05] 最大公约数
来源：http://tha.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://ktv.xuetiantiany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://slx.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bgd.haohaochexian.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gqx.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dcu.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dmj.ybcxt.top

Ruby: a.gcd(b)
来源：http://rxm.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gje.gaohongyu789.top

[N06] 判断回文字符串
来源：http://lcx.hywenlv.cn

Py:   s == s[::-1]
来源：http://qtc.jyoumei.cn

PHP:  $s === strrev($s);
来源：http://umm.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://bbt.shanyushiyangtech.top

TS:   s === [...s].reverse().join("")
来源：http://mdv.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zrz.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://txm.jlsjyb.cn

Ruby: s == s.reverse
来源：http://eoh.birdmap.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://koz.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://xyu.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rsm.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aal.52xcode.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rdy.chenlongwang.top

TS:   // 手写 Map<string, number>
来源：http://dky.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://xau.yongpay.top

Go:   // 手写 map[int]int
来源：http://nav.ppjwa.cn

Ruby: // 手写 Hash
来源：http://hnx.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wvt.xuanzx.com

[N08] 生成全排列
来源：http://ewa.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://bef.9152youxi.cn

PHP:  // 手写递归交换
来源：http://hho.sysykeji.top

JS:   // 手写回溯递归
来源：http://tjy.uphjek.com

TS:   // 手写回溯递归
来源：http://grs.vqdsnc.cn

Java: // 手写回溯递归
来源：http://izp.jinghuilouyu.cn

Go:   // 手写回溯递归
来源：http://amz.tianlin.xyz

Ruby: arr.permutation.to_a
来源：http://gpt.cqqwz.cn

C#:   // 手写回溯递归
来源：http://huk.hnxiangtu.top

[N09] 栈与队列
来源：http://svn.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://omb.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rcn.ctjpmb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wkz.bbcook.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qru.yvedp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vhi.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zsx.ppjwa.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tph.haohaochexian.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ogl.meibo888.top

[N10] 链表节点定义
来源：http://dyx.tanke756.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://slu.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://sda.snrcjt.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rfn.hnqzz.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fij.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://ydn.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://yuz.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uyl.c1oappe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nyk.nanxinkj.top

[N11] 二叉树中序遍历
来源：http://sfp.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lso.ydjk.org.cn


<!-- 参考信息 -->