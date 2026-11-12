代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qvv.zdbjq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nta.ywan-chungtsiang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ige.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qhi.pengpengdd.cyou

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ikz.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ycw.hnxiangtu.top

[K08] 二进制序列化（非 JSON）
来源：http://uht.yj202588.top

Py:   pickle.dumps(obj)
来源：http://pyv.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hjn.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://jxi.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://thi.fanxiaobao.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zkb.mhx1999.top

Go:   encoding/gob
来源：http://iys.yanxiufei.cn

Ruby: Marshal.dump(obj)
来源：http://ggh.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://utl.sufxvd.cn

================================================================================
来源：http://zda.hesvh.cn

L. 网络请求
来源：http://dwi.yanxiufei.cn

================================================================================
来源：http://xwz.tian-w.cn

[L01] 发送 GET 请求
来源：http://hwj.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ylm.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ysp.hywenlv.cn

JS:   await fetch(url)
来源：http://seo.chenjidiqi.icu

TS:   await fetch(url)
来源：http://tin.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://haf.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://icv.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rrs.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://igg.jqgfzy.top

[L02] 发送 POST JSON
来源：http://irq.yangfankeji.com

Py:   requests.post(url, json={"a": 1})
来源：http://qvp.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://itq.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iyw.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vqq.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://thn.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qcp.sufxvd.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xjj.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://esh.yonumen.top

[L03] 设置自定义请求头
来源：http://ewq.epnwcf.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tqb.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://spo.ctjpmb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pyn.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tyw.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://prk.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tlv.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hlj.andypj.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gry.quarkkingdee.top

[L04] 设置超时
来源：http://vnn.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://php.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mdl.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mqg.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tmi.nwbrower.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vgt.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://naq.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mhr.pycfn.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://shc.tianlin.xyz

[L05] 上传文件（multipart）
来源：http://pjg.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nxo.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://chr.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mgd.ehwqpu.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vsq.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ztx.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uio.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wtp.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aii.yuxming.cn

[L06] 解析响应为 JSON
来源：http://ken.c1oappe.top

Py:   resp.json()
来源：http://dyv.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://hsi.ybcxt.top

JS:   await resp.json()
来源：http://pjo.c1oappe.top

TS:   await resp.json()
来源：http://oyz.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ozi.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xev.haohaochexian.top

Ruby: JSON.parse(resp.body)
来源：http://fmi.epnwcf.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wtn.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://rsj.ppjwa.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dce.pengpengdd.cyou

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ukz.tanke756.top

JS:   resp.ok;  resp.status
来源：http://yof.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://ivl.ctjpmb.com

Java: resp.statusCode()
来源：http://dgp.smart0.xyz

Go:   resp.StatusCode
来源：http://jbs.daria6918.cn

Ruby: resp.code.to_i
来源：http://agy.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://wta.iojbl.cn

[L08] 并发请求多个地址
来源：http://yon.cqqwz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fmm.hesvh.cn

PHP:  curl_multi_init() 系列
来源：http://sqi.vehdjk.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zso.jinqigfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uvd.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jyf.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vbc.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jiv.cashguo.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aqv.jinghuilouyu.cn

================================================================================
来源：http://aea.nanxinkj.top

M. 命令行 / 进程 / 环境
来源：http://mel.jqgfzy.top

================================================================================
来源：http://mux.fengsongda.top

[M01] 读取命令行参数
来源：http://lnm.jinghuilouyu.cn

Py:   sys.argv[1:]
来源：http://qlg.zdqjudy.top

PHP:  $argv;  $argc;
来源：http://wdh.kuanghao11.cn

JS:   process.argv.slice(2)
来源：http://lsz.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://xvb.gogol.net.cn

Java: args 数组（main 方法参数）
来源：http://ldy.tanke756.top

Go:   os.Args[1:]
来源：http://uop.xinyue.icu

Ruby: ARGV
来源：http://csi.jqgfzy.top

C#:   args 数组（Main 方法参数）
来源：http://vrp.jinqigufen.top

[M02] 读取环境变量
来源：http://bqz.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://hyc.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hog.nanxuanxn.top

JS:   process.env.HOME
来源：http://qta.gogol.net.cn

TS:   process.env.HOME
来源：http://tdz.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://gkh.guowangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zuh.fanxiaobao.xyz

Ruby: ENV["HOME"]
来源：http://jol.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qzl.sweek.top

[M03] 执行外部命令
来源：http://qau.zhengqikj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pdv.zdbjq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gkm.fengsongda.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vty.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://inw.jiagoushi.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mhp.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bgg.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://emt.xylfe.cn

C#:   Process.Start("ls", "-l");
来源：http://zix.fktsv.cn

[M04] 获取当前工作目录
来源：http://cmf.smart0.xyz

Py:   os.getcwd()
来源：http://eaf.tarul.cn

PHP:  getcwd();
来源：http://xwp.guannengcc.top

JS:   process.cwd()
来源：http://ufx.sufxvd.cn

TS:   process.cwd()
来源：http://zqo.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://sbu.redwolf501.top

Go:   os.Getwd()
来源：http://yge.shanyushiyangkeji.top

Ruby: Dir.pwd
来源：http://isw.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://wsp.ctjpmb.com

[M05] 设置退出码
来源：http://mir.svipenyu.cn

Py:   sys.exit(1)
来源：http://bqc.kuanghao11.cn

PHP:  exit(1);
来源：http://pkx.iojbl.cn

JS:   process.exit(1)
来源：http://pjm.guannengcc.top

TS:   process.exit(1)
来源：http://gng.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://hgw.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://tqm.ppjwa.cn

Ruby: exit 1
来源：http://cjw.jianghu66.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dml.fanxiaobao.xyz

[M06] 向标准错误输出
来源：http://ldq.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://yel.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bym.guannengcc.top

JS:   console.error("err")
来源：http://wtb.gotoacloud.top

TS:   console.error("err")
来源：http://ejw.xinyue.icu

Java: System.err.println("err")
来源：http://rve.pycfn.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://erg.0kj1m.cn

Ruby: warn "err"
来源：http://tdo.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://fdu.daxiang520.top

[M07] 判断是否为主入口
来源：http://bay.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://vfi.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://svq.xinyue.icu

JS:   require.main === module
来源：http://xft.zhongyouzk.top

TS:   require.main === module
来源：http://tkt.pycfn.com

Java: public static void main(String[] args)
来源：http://wch.shuidangran.top

Go:   func main()
来源：http://apc.guowangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tsi.pycfn.com

C#:   static void Main(string[] args)
来源：http://yph.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://pnx.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://gic.dianchejie.cn

PHP:  PHP_OS;  phpversion();
来源：http://eaq.snrcjt.cn

JS:   process.platform;  process.version
来源：http://gmo.sysykeji.top

TS:   process.platform;  process.version
来源：http://nzs.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://moa.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://koz.jinghuilouyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kfi.nanxinkj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qlm.yuanzhike.top

================================================================================
来源：http://gxm.ivvv.top

N. 数据结构与算法
来源：http://rue.jqgfzy.top

================================================================================
来源：http://pdl.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://uzq.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://erw.hesvh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bje.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://obb.uphjek.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sfd.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vau.feifeiyinyue.top

Go:   sort.SearchInts(arr, x)
来源：http://tda.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xsk.shuidangran.top

C#:   Array.BinarySearch(arr, x)
来源：http://qlf.gotoacloud.top

[N02] 排序（工程实践用内置实现）
来源：http://mxk.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://wrx.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bpc.bjfxy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xqw.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xvv.daxiang520.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://deg.chenzaomai.com

Go:   slices.Sort(arr)
来源：http://bnt.hongshengwenyu.top

Ruby: arr.sort
来源：http://avm.ivvv.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mwo.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://omm.nwbrower.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zqj.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://lfr.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://scz.kuanghao11.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xil.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://htl.xziqi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ivc.daria6918.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ooc.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://ssg.sufxvd.cn

[N04] 斐波那契数列
来源：http://wbl.xuetiantiany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yvc.zhijiandao.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qyi.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qdy.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://krm.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ofs.jianghu66.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vkb.nwbrower.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cjy.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://afz.daria6918.cn

[N05] 最大公约数
来源：http://ift.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://cpg.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tou.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dwd.quarkkingdee.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kzf.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ija.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qsw.yvedp.cn

Ruby: a.gcd(b)
来源：http://jfd.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kle.hfpthk.cn

[N06] 判断回文字符串
来源：http://cro.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://wwu.bjfxy.top

PHP:  $s === strrev($s);
来源：http://ykf.yj20258888.top

JS:   s === [...s].reverse().join("")
来源：http://imc.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://hsy.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gzt.guannengcc.top

Go:   // 双指针从两端比较
来源：http://ofu.dashuyun.cn

Ruby: s == s.reverse
来源：http://sig.jinghuilouyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://niq.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://foi.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gaa.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yow.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cpu.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://ijs.gogol.net.cn

Java: // 手写 HashMap
来源：http://rdr.aizwys.cn

Go:   // 手写 map[int]int
来源：http://orc.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://leg.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gst.yj20258888.top

[N08] 生成全排列
来源：http://mst.yj202588.top

Py:   itertools.permutations(arr)
来源：http://zio.fzhhl.top

PHP:  // 手写递归交换
来源：http://olh.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://wgy.yj20258888.top

TS:   // 手写回溯递归
来源：http://vjg.yuanzhike.top

Java: // 手写回溯递归
来源：http://xmn.sufxvd.cn

Go:   // 手写回溯递归
来源：http://mrn.jianghu66.top

Ruby: arr.permutation.to_a
来源：http://cqh.kuanghao11.cn

C#:   // 手写回溯递归
来源：http://dqo.jyoumei.cn

[N09] 栈与队列
来源：http://lsv.xinyue.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sgh.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nja.jianghu66.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ldg.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rji.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qxj.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kwx.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://glf.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rrm.jqgfzy.top

[N10] 链表节点定义
来源：http://vqa.ppjwa.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fnb.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://prq.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wpc.shzxlz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rxa.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://kit.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://mip.redwolf501.top

Ruby: Node = Struct.new(:v, :next)
来源：http://khi.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://rwd.hcnkem.com

[N11] 二叉树中序遍历
来源：http://jeq.meibo888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hdx.0kj1m.cn

PHP:  // 手写递归函数
来源：http://kwa.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uxa.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ism.quarkkingdee.top

Java: // 手写递归
来源：http://php.shuidangran.top

Go:   // 手写递归
来源：http://wng.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dfh.svipenyu.cn

C#:   // 手写递归
来源：http://gnu.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tan.chenlongwang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yda.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tky.epnwcf.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mdc.yuanzhike.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rav.tarul.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kgp.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xrb.zdqjudy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hrl.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kaf.nanxinkj.top

================================================================================
来源：http://qjj.xylfe.cn

O. 并发与异步
来源：http://qns.yuanzhike.top

================================================================================
来源：http://lkz.iojbl.cn

[O01] 启动一个线程
来源：http://jit.jqgufenzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zcx.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nfi.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uoz.ctjpmb.com

TS:   // 同 JS
来源：http://rlr.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://ptk.gotoacloud.top

Go:   go f()
来源：http://zop.tianlin.xyz

Ruby: Thread.new { f }
来源：http://xev.nwbrower.top

C#:   Task.Run(() => F());
来源：http://qvs.cqqwz.cn

[O02] 使用线程池
来源：http://wof.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rls.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fad.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://xfy.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://gax.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://ggo.xinyue.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pqt.fengsongda.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ysl.meibo888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cbm.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://bzk.hysaishi.cn

Py:   with lock: shared += 1
来源：http://qno.sysykeji.top

PHP:  // 用 flock() 做文件锁
来源：http://mgc.yonumen.top


<!-- 参考信息 -->