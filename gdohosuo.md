代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rop.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://foj.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tzx.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zhv.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://njz.xziqi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hho.zhengqikj.top

[K08] 二进制序列化（非 JSON）
来源：http://nqi.yj202588.top

Py:   pickle.dumps(obj)
来源：http://ull.nwbrower.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ldn.guowangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://pub.jyoumei.cn

TS:   v8.serialize(obj)        // Node
来源：http://vlb.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://abk.aizwys.cn

Go:   encoding/gob
来源：http://jte.ydjk.org.cn

Ruby: Marshal.dump(obj)
来源：http://vaw.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jwz.epnwcf.com

================================================================================
来源：http://jer.sxryk.cn

L. 网络请求
来源：http://oon.nanxuanxn.top

================================================================================
来源：http://pac.jiagoushi.top

[L01] 发送 GET 请求
来源：http://yho.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://koy.sysykeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gjo.jiagoushi.top

JS:   await fetch(url)
来源：http://ngw.wangdashe.top

TS:   await fetch(url)
来源：http://cxf.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kaf.kuanghao11.cn

Go:   resp, err := http.Get(url)
来源：http://lpm.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rqx.cucudq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://chv.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://skm.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://axx.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vne.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hpb.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wiy.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://efj.zdbjq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wmx.quarkkingdee.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fhi.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://obo.yangfankeji.com

[L03] 设置自定义请求头
来源：http://pya.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ihi.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ycb.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qdy.vqdsnc.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rdt.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rhn.chenzaomai.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yte.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kjw.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ztn.yj20258.top

[L04] 设置超时
来源：http://fan.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://hvi.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rlw.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jvr.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://omc.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kqg.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kig.316326.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://syd.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uts.yvedp.cn

[L05] 上传文件（multipart）
来源：http://jrf.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uiq.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pez.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hzd.jianghu66.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bnz.jinghuilouyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lpg.jinqigufen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pnm.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nvx.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fni.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://bnb.vehdjk.com

Py:   resp.json()
来源：http://irm.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://txm.hesvh.cn

JS:   await resp.json()
来源：http://wqk.yj202588.top

TS:   await resp.json()
来源：http://lmd.gaohongyu789.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iux.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qes.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://okz.zdqjudy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uxu.nanxuanxn.top

[L07] 处理 HTTP 状态码
来源：http://irp.zhoulong.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nvk.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://imd.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://eey.yonumen.top

TS:   resp.ok;  resp.status
来源：http://gog.ivvv.top

Java: resp.statusCode()
来源：http://qle.xinyue.icu

Go:   resp.StatusCode
来源：http://ilw.snrcjt.cn

Ruby: resp.code.to_i
来源：http://nbm.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://yqj.guannengcc.top

[L08] 并发请求多个地址
来源：http://tpt.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kxa.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://azx.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lwt.vehdjk.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bgq.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pmy.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eqm.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vhs.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ulc.ydjk.org.cn

================================================================================
来源：http://ojb.ydzc1.top

M. 命令行 / 进程 / 环境
来源：http://ctx.hfpthk.cn

================================================================================
来源：http://vav.xziqi.cn

[M01] 读取命令行参数
来源：http://jfi.jqgfzy.top

Py:   sys.argv[1:]
来源：http://xlm.xylfe.cn

PHP:  $argv;  $argc;
来源：http://icx.tarul.cn

JS:   process.argv.slice(2)
来源：http://kpw.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://hfo.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://xjs.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://suf.nanxinkj.top

Ruby: ARGV
来源：http://hck.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://gig.pengpengdd.cyou

[M02] 读取环境变量
来源：http://gle.vqdsnc.cn

Py:   os.environ.get("HOME")
来源：http://kvr.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fsu.ydjk.org.cn

JS:   process.env.HOME
来源：http://czi.hesvh.cn

TS:   process.env.HOME
来源：http://siu.aibaodan.cn

Java: System.getenv("HOME")
来源：http://mkv.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mzu.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://fqq.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://img.yfazqb.com

[M03] 执行外部命令
来源：http://oqk.fktsv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://goy.yonumen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xhu.hysaishi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lzb.hnxiangtu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xhg.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://coq.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ryt.yuxming.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rja.sxryk.cn

C#:   Process.Start("ls", "-l");
来源：http://hbo.shuidangran.top

[M04] 获取当前工作目录
来源：http://vmc.nwbrower.top

Py:   os.getcwd()
来源：http://usf.snrcjt.cn

PHP:  getcwd();
来源：http://vog.bjfxy.top

JS:   process.cwd()
来源：http://ljd.dianchejie.cn

TS:   process.cwd()
来源：http://fna.zhoulong.xyz

Java: Path.of("").toAbsolutePath()
来源：http://eeq.ivvv.top

Go:   os.Getwd()
来源：http://fpv.xylfe.cn

Ruby: Dir.pwd
来源：http://vkx.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lxf.zdqjudy.top

[M05] 设置退出码
来源：http://gkd.shzxlz.cn

Py:   sys.exit(1)
来源：http://aok.ehwqpu.com

PHP:  exit(1);
来源：http://mfw.cqqwz.cn

JS:   process.exit(1)
来源：http://fgp.iojbl.cn

TS:   process.exit(1)
来源：http://wzs.sxryk.cn

Java: System.exit(1)
来源：http://klv.vehdjk.com

Go:   os.Exit(1)
来源：http://cns.dianchejie.cn

Ruby: exit 1
来源：http://jbx.xuetiantiany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://woh.xylfe.cn

[M06] 向标准错误输出
来源：http://mpq.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://rxa.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kcd.pengpengdd.cyou

JS:   console.error("err")
来源：http://bgf.yfazqb.com

TS:   console.error("err")
来源：http://kzf.cdnleiting.top

Java: System.err.println("err")
来源：http://neg.vqdsnc.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://atm.haohaochexian.top

Ruby: warn "err"
来源：http://xat.guannengcc.top

C#:   Console.Error.WriteLine("err")
来源：http://pci.redwolf501.top

[M07] 判断是否为主入口
来源：http://sbx.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://bsy.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fxa.zhoulong.xyz

JS:   require.main === module
来源：http://tsi.xuanzx.com

TS:   require.main === module
来源：http://zuh.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://hjw.chenzaomai.com

Go:   func main()
来源：http://sez.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://phi.daria6918.cn

C#:   static void Main(string[] args)
来源：http://mqs.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://zxu.birdmap.top

Py:   platform.system();  platform.python_version()
来源：http://fof.yangfankeji.com

PHP:  PHP_OS;  phpversion();
来源：http://kpj.9152youxi.cn

JS:   process.platform;  process.version
来源：http://wmw.jiagoushi.top

TS:   process.platform;  process.version
来源：http://cbj.xylfe.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tgt.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dla.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fqn.feifeiyinyue.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hbl.tarul.cn

================================================================================
来源：http://icp.ydzc1.top

N. 数据结构与算法
来源：http://hfs.zhaomingkeji.xyz

================================================================================
来源：http://ypn.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://qpl.guowangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://lba.uphjek.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rwn.xuetiantiany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jrs.ydzc1.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cxo.gogol.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yrn.hongshengwenyu.top

Go:   sort.SearchInts(arr, x)
来源：http://jxe.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pbd.yfazqb.com

C#:   Array.BinarySearch(arr, x)
来源：http://gor.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://rof.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://coc.ybcxt.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mwx.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://khs.cdnleiting.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kud.nanxuanxn.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tnu.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://lbm.zhijiandao.cn

Ruby: arr.sort
来源：http://cyf.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://euq.sysykeji.top

[N03] 快速排序（分治示例）
来源：http://ulb.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vhp.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://inc.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qyf.sweek.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bpn.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hpq.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xvt.chenjidiqi.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hnj.shanyushiyangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://ozw.mhx1999.top

[N04] 斐波那契数列
来源：http://tny.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uke.wangdashe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rpt.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lsr.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pfg.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wkx.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kip.bjfxy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jva.yvedp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gqr.shuidangran.top

[N05] 最大公约数
来源：http://uxp.havefunace.top

Py:   math.gcd(a, b)
来源：http://lrw.hfpthk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://edd.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ohz.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zzg.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yos.sysykeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yey.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://vwm.pengpengdd.cyou

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hdb.cheryme.top

[N06] 判断回文字符串
来源：http://xgf.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://gxg.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://wvf.zycfv.cn

JS:   s === [...s].reverse().join("")
来源：http://nvn.andypj.xyz

TS:   s === [...s].reverse().join("")
来源：http://oyu.yongpay.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tvh.epnwcf.com

Go:   // 双指针从两端比较
来源：http://sdm.hnxiangtu.top

Ruby: s == s.reverse
来源：http://oax.jqgufenzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://suo.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://saz.fktsv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ykv.xylfe.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xsk.fengsongda.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fux.hongshengwenyu.top

TS:   // 手写 Map<string, number>
来源：http://iwi.xingfuxueyuan.xyz

Java: // 手写 HashMap
来源：http://boq.hnxiangtu.top

Go:   // 手写 map[int]int
来源：http://ozd.chenlongwang.top

Ruby: // 手写 Hash
来源：http://ptj.316326.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://pfp.hysaishi.cn

[N08] 生成全排列
来源：http://fzi.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://gcr.yangfankeji.com

PHP:  // 手写递归交换
来源：http://lnl.shanyushiyangtech.top

JS:   // 手写回溯递归
来源：http://qqe.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://poc.andypj.xyz

Java: // 手写回溯递归
来源：http://mik.gotoacloud.top

Go:   // 手写回溯递归
来源：http://ncf.sweek.top

Ruby: arr.permutation.to_a
来源：http://gtx.yangfankeji.com

C#:   // 手写回溯递归
来源：http://ibs.shuidangran.top

[N09] 栈与队列
来源：http://gae.shangyingyoupin.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kvg.yj20258.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xlu.sjlbkw.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pmh.chenzaomai.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bvz.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zhw.cqqwz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://myx.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ugn.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hlu.tian-w.cn

[N10] 链表节点定义
来源：http://iss.ehwqpu.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xje.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nkq.zycfv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://upi.zdqjudy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xyu.ivvv.top

Java: class Node { int v; Node next; }
来源：http://kcq.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://pdl.cashguo.top

Ruby: Node = Struct.new(:v, :next)
来源：http://oqk.zdbjq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rko.cashguo.top

[N11] 二叉树中序遍历
来源：http://upm.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gfh.nwbrower.top

PHP:  // 手写递归函数
来源：http://uih.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hsy.yangfankeji.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://akq.gogol.net.cn

Java: // 手写递归
来源：http://gxw.zhaomingkeji.xyz

Go:   // 手写递归
来源：http://moj.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tgk.aibaodan.cn

C#:   // 手写递归
来源：http://coj.redwolf501.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rcp.zhoulong.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ayj.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vyv.chenlongwang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kke.gotoacloud.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bzt.yongpay.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://awx.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bqp.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kpz.zhengqikj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hce.sjlbkw.cn

================================================================================
来源：http://zua.yfazqb.com

O. 并发与异步
来源：http://zxt.wangshuangyany.cn

================================================================================
来源：http://buu.svipenyu.cn

[O01] 启动一个线程
来源：http://msv.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qen.fktsv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yxa.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://upr.fzhhl.top

TS:   // 同 JS
来源：http://lej.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://rai.cqqwz.cn

Go:   go f()
来源：http://ikx.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://fqi.cucudq.cn

C#:   Task.Run(() => F());
来源：http://bfg.yuxming.cn

[O02] 使用线程池
来源：http://vwy.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wwo.feifeiyinyue.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ifd.sjlbkw.cn

JS:   // worker_threads 线程池
来源：http://vqm.xylfe.cn

TS:   // worker_threads 线程池
来源：http://dym.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://zfj.hongshengwenyu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://osh.xylfe.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bug.birdmap.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dbr.zhaomingkeji.xyz

[O03] 加锁保护共享数据
来源：http://ypa.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://idh.cqqwz.cn

PHP:  // 用 flock() 做文件锁
来源：http://qjr.sxryk.cn


<!-- 参考信息 -->