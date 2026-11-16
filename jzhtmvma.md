代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://juk.birdmap.top

[K07] 进制转换
来源：http://oda.tarul.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tuz.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wcl.yuxming.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wmg.chenzaomai.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qhc.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hfe.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ews.hesvh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://enl.sysykeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kvu.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://kdc.tian-w.cn

Py:   pickle.dumps(obj)
来源：http://nyf.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cpx.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://rvx.gotoacloud.top

TS:   v8.serialize(obj)        // Node
来源：http://euo.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yek.hammf.cn

Go:   encoding/gob
来源：http://jxd.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://ioo.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jlm.svipenyu.cn

================================================================================
来源：http://gnl.tanke756.top

L. 网络请求
来源：http://lsn.epnwcf.com

================================================================================
来源：http://mbf.xingfuxueyuan.xyz

[L01] 发送 GET 请求
来源：http://rxe.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vrd.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xvv.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://lks.hnxiangtu.top

TS:   await fetch(url)
来源：http://dpx.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ums.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://qyu.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://moo.cqqwz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cxq.yuanzhike.top

[L02] 发送 POST JSON
来源：http://vlm.jyoumei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://iue.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hfl.vehdjk.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eaa.svipenyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qju.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zhh.kuanghao11.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cqq.vehdjk.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hmb.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nxt.zhengqikj.top

[L03] 设置自定义请求头
来源：http://dac.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jmm.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xgn.chenlongwang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ilq.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kqp.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hkd.jqgfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wjc.hnqzz.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://elk.zhaomingkeji.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wxo.tanke756.top

[L04] 设置超时
来源：http://hgk.jinyuanbaomall.cn

Py:   requests.get(url, timeout=5)
来源：http://iqp.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ceq.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ehw.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kes.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gay.jlsjyb.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://git.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jmm.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://elv.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://lja.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eto.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://odq.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ppp.feifeiyinyue.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gou.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rry.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xgm.tianlin.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ipf.wangdashe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gcw.uphjek.com

[L06] 解析响应为 JSON
来源：http://ivr.wangdashe.top

Py:   resp.json()
来源：http://cpf.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://prg.zdbjq.cn

JS:   await resp.json()
来源：http://pjs.yongpay.top

TS:   await resp.json()
来源：http://zce.ehwqpu.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vmj.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bkp.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://fdu.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gda.vqdsnc.cn

[L07] 处理 HTTP 状态码
来源：http://smr.vehdjk.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ogr.shuidangran.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://adl.ydzc1.top

JS:   resp.ok;  resp.status
来源：http://yki.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://pro.ehwqpu.com

Java: resp.statusCode()
来源：http://okf.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://wql.aibaodan.cn

Ruby: resp.code.to_i
来源：http://vlc.sjlbkw.cn

C#:   (int)resp.StatusCode
来源：http://jfd.52xcode.cn

[L08] 并发请求多个地址
来源：http://xtb.sufxvd.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gkv.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://azi.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rwq.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vfa.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qms.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kew.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bgl.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dhu.fehbvm.com

================================================================================
来源：http://vke.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://wfd.ydjk.org.cn

================================================================================
来源：http://rvr.hywenlv.cn

[M01] 读取命令行参数
来源：http://mqz.fzhhl.top

Py:   sys.argv[1:]
来源：http://ucj.gzhubu.top

PHP:  $argv;  $argc;
来源：http://xvc.ydzc1.top

JS:   process.argv.slice(2)
来源：http://zmy.andypj.xyz

TS:   process.argv.slice(2)
来源：http://nkg.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://lzc.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://met.snrcjt.cn

Ruby: ARGV
来源：http://tmb.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://vpx.svipenyu.cn

[M02] 读取环境变量
来源：http://cdy.316326.xyz

Py:   os.environ.get("HOME")
来源：http://zjc.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ypr.sysykeji.top

JS:   process.env.HOME
来源：http://kvb.zhiwuduotai.top

TS:   process.env.HOME
来源：http://zbf.svipenyu.cn

Java: System.getenv("HOME")
来源：http://mmd.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rfu.yanxiufei.cn

Ruby: ENV["HOME"]
来源：http://gkq.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yyp.smart0.xyz

[M03] 执行外部命令
来源：http://fdf.jlsjyb.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kpb.uphjek.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jov.vehdjk.com

JS:   child_process.execSync("ls -l").toString()
来源：http://lha.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dzi.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fos.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wvc.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xdb.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://jdj.chenzaomai.com

[M04] 获取当前工作目录
来源：http://fjg.cashguo.top

Py:   os.getcwd()
来源：http://xqc.zhiwuduotai.top

PHP:  getcwd();
来源：http://vzf.andypj.xyz

JS:   process.cwd()
来源：http://dug.yvedp.cn

TS:   process.cwd()
来源：http://uhn.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://rdd.yj20258888.top

Go:   os.Getwd()
来源：http://ual.bbcook.cn

Ruby: Dir.pwd
来源：http://sum.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://fmc.aibaodan.cn

[M05] 设置退出码
来源：http://avc.xziqi.cn

Py:   sys.exit(1)
来源：http://tpq.xylfe.cn

PHP:  exit(1);
来源：http://lil.tarul.cn

JS:   process.exit(1)
来源：http://fbe.vqdsnc.cn

TS:   process.exit(1)
来源：http://gzz.vehdjk.com

Java: System.exit(1)
来源：http://qvr.ppjwa.cn

Go:   os.Exit(1)
来源：http://wbm.tian-w.cn

Ruby: exit 1
来源：http://tvs.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tms.chenjidiqi.icu

[M06] 向标准错误输出
来源：http://pqj.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://ozm.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ema.meibo888.top

JS:   console.error("err")
来源：http://tgu.chenjidiqi.icu

TS:   console.error("err")
来源：http://xhi.zhixingplan.top

Java: System.err.println("err")
来源：http://jbw.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jaj.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://qub.jqgfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://uap.yj202588.top

[M07] 判断是否为主入口
来源：http://etf.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://nfm.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://htv.shanyushiyangkeji.top

JS:   require.main === module
来源：http://bcy.tarul.cn

TS:   require.main === module
来源：http://kra.cheryme.top

Java: public static void main(String[] args)
来源：http://ftw.shangyingyoupin.top

Go:   func main()
来源：http://uzm.9152youxi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tmt.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://ydy.ivvv.top

[M08] 获取系统与运行时信息
来源：http://upm.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://zuo.xinyue.icu

PHP:  PHP_OS;  phpversion();
来源：http://jcy.sufxvd.cn

JS:   process.platform;  process.version
来源：http://pdc.vehdjk.com

TS:   process.platform;  process.version
来源：http://tsj.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xuq.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xfj.pycfn.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jkv.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://jlg.pengpengdd.cyou

================================================================================
来源：http://hfl.hnxiangtu.top

N. 数据结构与算法
来源：http://jnd.dashuyun.cn

================================================================================
来源：http://bbg.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://mnm.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://inl.sjlbkw.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ril.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://elz.gotoacloud.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://knb.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://bkp.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://dyu.pengpengdd.cyou

Ruby: arr.bsearch { |e| e >= x }
来源：http://dsh.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://xgv.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://cnw.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://vzc.fzhhl.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xec.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://xrh.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ylu.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jgr.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://liw.nanxinkj.top

Ruby: arr.sort
来源：http://pru.bjfxy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qjy.jqgfzy.top

[N03] 快速排序（分治示例）
来源：http://gvy.zhijiandao.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://her.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://roc.yueranfly.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ffl.kuanghao11.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iju.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ufd.zycfv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lwm.sufxvd.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xov.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://hqh.redwolf501.top

[N04] 斐波那契数列
来源：http://wrn.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://spg.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fwd.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ahv.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zwy.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hrj.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hiu.jianghu66.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kro.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://phi.ydzc1.top

[N05] 最大公约数
来源：http://rih.fengsongda.top

Py:   math.gcd(a, b)
来源：http://ljg.daxiang520.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://spp.chenzaomai.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ndz.cqqwz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mdh.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://llv.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://imo.yj20258888.top

Ruby: a.gcd(b)
来源：http://nkd.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fbu.xuanzx.com

[N06] 判断回文字符串
来源：http://nug.zdbjq.cn

Py:   s == s[::-1]
来源：http://rwe.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://quo.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://qux.jinqigfzy.top

TS:   s === [...s].reverse().join("")
来源：http://hez.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://olr.cucudq.cn

Go:   // 双指针从两端比较
来源：http://kxc.tarul.cn

Ruby: s == s.reverse
来源：http://mmh.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://prg.yj202588.top

[N07] 两数之和（返回下标）
来源：http://jgk.hnxiangtu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uzb.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zyy.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gsg.snrcjt.cn

TS:   // 手写 Map<string, number>
来源：http://vlh.gzhubu.top

Java: // 手写 HashMap
来源：http://izu.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://hrf.jinghuilouyu.cn

Ruby: // 手写 Hash
来源：http://gnh.chenzaomai.com

C#:   // 手写 Dictionary<int, int>
来源：http://lrs.xylfe.cn

[N08] 生成全排列
来源：http://pjg.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://btk.yueranfly.top

PHP:  // 手写递归交换
来源：http://iut.yvedp.cn

JS:   // 手写回溯递归
来源：http://epx.jiagoushi.top

TS:   // 手写回溯递归
来源：http://jmr.meibo888.top

Java: // 手写回溯递归
来源：http://wsa.daria6918.cn

Go:   // 手写回溯递归
来源：http://tcn.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://qpr.aibaodan.cn

C#:   // 手写回溯递归
来源：http://jhk.birdmap.top

[N09] 栈与队列
来源：http://mnc.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ivw.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xje.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://szs.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://msc.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pag.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://isk.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lmg.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zcn.mhx1999.top

[N10] 链表节点定义
来源：http://gll.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qjv.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://mbj.zhengqikj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pjo.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zrv.yuxming.cn

Java: class Node { int v; Node next; }
来源：http://iox.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://wym.vqdsnc.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lwo.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jcb.chenlongwang.top

[N11] 二叉树中序遍历
来源：http://gsc.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wcy.sufxvd.cn

PHP:  // 手写递归函数
来源：http://qng.smart0.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tdb.jinghuilouyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mzu.yonumen.top

Java: // 手写递归
来源：http://esk.zhongyouzk.top

Go:   // 手写递归
来源：http://vxw.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vhn.hywenlv.cn

C#:   // 手写递归
来源：http://hkw.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qqc.svipenyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ptm.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ujx.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ziw.ctjpmb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lql.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jpq.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ojt.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hlo.zdbjq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xxi.jinghuilouyu.cn

================================================================================
来源：http://icd.zhijiandao.cn

O. 并发与异步
来源：http://rzt.yuxming.cn

================================================================================
来源：http://rlh.iojbl.cn

[O01] 启动一个线程
来源：http://whc.zdqjudy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gjn.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oso.fehbvm.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://etm.hywenlv.cn

TS:   // 同 JS
来源：http://our.epnwcf.com

Java: new Thread(() -> f()).start()
来源：http://evl.shangyingyoupin.top

Go:   go f()
来源：http://rhh.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://wuq.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://edk.meibo888.top

[O02] 使用线程池
来源：http://ocu.jlsjyb.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mxi.0kj1m.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dqz.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://zlx.xuetiantiany.cn

TS:   // worker_threads 线程池
来源：http://bxc.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://egi.sxryk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://psk.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mpa.birdmap.top


<!-- 参考信息 -->