代发 wailian999

TS:   JSON.parse(s)
来源：http://iud.pengpengdd.cyou

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dzk.cheryme.top

Go:   json.Unmarshal(data, &v)
来源：http://izd.andypj.xyz

Ruby: JSON.parse(s)
来源：http://scu.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qgg.hongshengwenyu.top

[K03] JSON 美化输出（带缩进）
来源：http://edd.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bdj.jianghu66.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yxe.meibo888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lti.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mbx.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bhp.hcnkem.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tgx.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://iqg.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dhg.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://zgl.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xzq.tian-w.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mcs.nwbrower.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://umy.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ctx.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xue.hywenlv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://szv.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cpt.uphjek.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qgv.daria6918.cn

[K05] 深拷贝对象
来源：http://ary.xuetiantiany.cn

Py:   copy.deepcopy(obj)
来源：http://kuv.fehbvm.com

PHP:  unserialize(serialize($obj));
来源：http://qnk.shzxlz.cn

JS:   structuredClone(obj)
来源：http://ljb.zhoulong.xyz

TS:   structuredClone(obj)
来源：http://vtg.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ktg.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ttr.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lgs.yvedp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vxe.epnwcf.com

[K06] 解析 URL 查询串
来源：http://zmw.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jju.hywenlv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://axy.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qqa.daria6918.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rnb.pengpengdd.cyou

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kng.snrcjt.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tyr.wangshuangyany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kqd.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zdh.dianchejie.cn

[K07] 进制转换
来源：http://hzn.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://htg.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vgz.hcnkem.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nsn.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wgm.gzhubu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://psp.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zvq.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://juf.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rgz.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://fbl.jqgfzy.top

Py:   pickle.dumps(obj)
来源：http://phu.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://wiq.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://era.mhx1999.top

TS:   v8.serialize(obj)        // Node
来源：http://qbq.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://adh.smart0.xyz

Go:   encoding/gob
来源：http://rvl.nanxinkj.top

Ruby: Marshal.dump(obj)
来源：http://uxg.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nhf.fehbvm.com

================================================================================
来源：http://drw.yanxiufei.cn

L. 网络请求
来源：http://sxp.zhaomingkeji.xyz

================================================================================
来源：http://awg.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://eel.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://evj.epnwcf.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uhs.fengsongda.top

JS:   await fetch(url)
来源：http://xbj.wangshuangyany.cn

TS:   await fetch(url)
来源：http://bmi.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://urg.yuxming.cn

Go:   resp, err := http.Get(url)
来源：http://wnm.uphjek.com

Ruby: Net::HTTP.get(URI(url))
来源：http://tin.hywenlv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://usr.hfpthk.cn

[L02] 发送 POST JSON
来源：http://pro.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://lej.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jkv.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eas.fengsongda.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zns.yj202588.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pjh.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qaw.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nhc.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ior.zhongyouzk.top

[L03] 设置自定义请求头
来源：http://uzh.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://slq.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tyl.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://drb.vehdjk.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://igj.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vnz.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uwc.iojbl.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vbp.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vpn.sufxvd.cn

[L04] 设置超时
来源：http://elb.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://lpl.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dzl.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kov.bbcook.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://obl.zycfv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hph.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uow.yj20258888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uki.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pkb.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://jyr.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nzr.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xtm.birdmap.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ake.dashuyun.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sam.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fcj.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tee.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sti.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://noe.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://gyp.jqgufenzy.top

Py:   resp.json()
来源：http://vvj.aizwys.cn

PHP:  json_decode($body, true);
来源：http://xdf.yj20258888.top

JS:   await resp.json()
来源：http://vbr.zhengqikj.top

TS:   await resp.json()
来源：http://cxd.jqgfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nfy.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gzn.zhaomingkeji.xyz

Ruby: JSON.parse(resp.body)
来源：http://wmz.jlsjyb.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fzq.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://psk.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tjj.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aps.tanke756.top

JS:   resp.ok;  resp.status
来源：http://avf.yongpay.top

TS:   resp.ok;  resp.status
来源：http://aaz.xuetiantiany.cn

Java: resp.statusCode()
来源：http://zsf.ydjk.org.cn

Go:   resp.StatusCode
来源：http://pcn.guowangkeji.top

Ruby: resp.code.to_i
来源：http://kip.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://yje.zhixingplan.top

[L08] 并发请求多个地址
来源：http://tjz.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://izp.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://uwe.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bru.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cli.nwbrower.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://taw.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yni.yonumen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oic.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eht.haohaochexian.top

================================================================================
来源：http://ghf.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://vgz.cdnleiting.top

================================================================================
来源：http://rdt.shzxlz.cn

[M01] 读取命令行参数
来源：http://tzt.yvedp.cn

Py:   sys.argv[1:]
来源：http://gws.sweek.top

PHP:  $argv;  $argc;
来源：http://zeg.tanke756.top

JS:   process.argv.slice(2)
来源：http://eoi.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://rqh.ivvv.top

Java: args 数组（main 方法参数）
来源：http://mmx.jqgfzy.top

Go:   os.Args[1:]
来源：http://heb.0kj1m.cn

Ruby: ARGV
来源：http://yza.jinqigufen.top

C#:   args 数组（Main 方法参数）
来源：http://uab.yanxiufei.cn

[M02] 读取环境变量
来源：http://mrg.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://rmg.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zje.iojbl.cn

JS:   process.env.HOME
来源：http://dvx.aizwys.cn

TS:   process.env.HOME
来源：http://ubf.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://uuo.havefunace.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uvi.yvedp.cn

Ruby: ENV["HOME"]
来源：http://nvl.chenjidiqi.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ely.fanxiaobao.xyz

[M03] 执行外部命令
来源：http://avh.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gsy.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jlf.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://aya.mhx1999.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jzn.zhoulong.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qao.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cup.zhixingplan.top

Ruby: system("ls -l");  `ls -l`
来源：http://ghg.xylfe.cn

C#:   Process.Start("ls", "-l");
来源：http://bpn.kuanghao11.cn

[M04] 获取当前工作目录
来源：http://qgn.xuanzx.com

Py:   os.getcwd()
来源：http://nom.yueranfly.top

PHP:  getcwd();
来源：http://ssn.fzhhl.top

JS:   process.cwd()
来源：http://kdy.jqgfzy.top

TS:   process.cwd()
来源：http://zpl.andypj.xyz

Java: Path.of("").toAbsolutePath()
来源：http://fsu.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://chw.hammf.cn

Ruby: Dir.pwd
来源：http://dur.dashuyun.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bnw.zhoulong.xyz

[M05] 设置退出码
来源：http://boq.yueranfly.top

Py:   sys.exit(1)
来源：http://loq.gzhubu.top

PHP:  exit(1);
来源：http://ywn.cucudq.cn

JS:   process.exit(1)
来源：http://ady.zhijiandao.cn

TS:   process.exit(1)
来源：http://zmz.cqqwz.cn

Java: System.exit(1)
来源：http://pao.aizwys.cn

Go:   os.Exit(1)
来源：http://vwa.gaohongyu789.top

Ruby: exit 1
来源：http://ngx.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jxz.hfpthk.cn

[M06] 向标准错误输出
来源：http://vcd.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://sxs.xziqi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://duq.hnxiangtu.top

JS:   console.error("err")
来源：http://fwp.jinyuanbaomall.cn

TS:   console.error("err")
来源：http://euk.gaohongyu789.top

Java: System.err.println("err")
来源：http://nlr.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://srz.cashguo.top

Ruby: warn "err"
来源：http://rwv.wangshuangyany.cn

C#:   Console.Error.WriteLine("err")
来源：http://ozu.shuidangran.top

[M07] 判断是否为主入口
来源：http://cev.pycfn.com

Py:   if __name__ == "__main__":
来源：http://jfv.kuanghao11.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ega.tianlin.xyz

JS:   require.main === module
来源：http://dsi.tianlin.xyz

TS:   require.main === module
来源：http://rux.hesvh.cn

Java: public static void main(String[] args)
来源：http://vkl.jlsjyb.cn

Go:   func main()
来源：http://dgx.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://flh.hesvh.cn

C#:   static void Main(string[] args)
来源：http://opb.gogol.net.cn

[M08] 获取系统与运行时信息
来源：http://rrr.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://bxv.uphjek.com

PHP:  PHP_OS;  phpversion();
来源：http://wdo.jianghu66.top

JS:   process.platform;  process.version
来源：http://kfk.yongpay.top

TS:   process.platform;  process.version
来源：http://aal.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mpa.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dvi.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://obl.dianchejie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wwa.zhiwuduotai.top

================================================================================
来源：http://qoa.cucudq.cn

N. 数据结构与算法
来源：http://zfz.jyoumei.cn

================================================================================
来源：http://uga.cucudq.cn

[N01] 二分查找（有序数组）
来源：http://blj.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pip.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pci.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://okq.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://thy.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ier.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://uqk.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gyi.yongpay.top

C#:   Array.BinarySearch(arr, x)
来源：http://ayq.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://yjy.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://qjs.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ian.cqqwz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jie.fktsv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://quf.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lxi.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://epr.meibo888.top

Ruby: arr.sort
来源：http://ond.jinyuanbaomall.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lmy.cheryme.top

[N03] 快速排序（分治示例）
来源：http://niv.nanxuanxn.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zfd.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://cgz.shuidangran.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xst.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pvj.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qzx.birdmap.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ajr.feifeiyinyue.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vau.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://jkc.bbcook.cn

[N04] 斐波那契数列
来源：http://jqz.yfazqb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rig.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gue.aibaodan.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dsy.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kez.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://trg.nwbrower.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wqn.zhiwuduotai.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ilr.xuetiantiany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wvn.shangyingyoupin.top

[N05] 最大公约数
来源：http://oym.316326.xyz

Py:   math.gcd(a, b)
来源：http://zej.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nzy.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://odh.smart0.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ptd.pycfn.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kfr.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vbg.jqgfzy.top

Ruby: a.gcd(b)
来源：http://whe.9152youxi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qlq.shzxlz.cn

[N06] 判断回文字符串
来源：http://ilm.hcnkem.com

Py:   s == s[::-1]
来源：http://wae.cheryme.top

PHP:  $s === strrev($s);
来源：http://jdb.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://wuh.hongshengwenyu.top

TS:   s === [...s].reverse().join("")
来源：http://lzd.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qzt.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://wsr.yj20258.top

Ruby: s == s.reverse
来源：http://vip.gzhubu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tfy.0kj1m.cn

[N07] 两数之和（返回下标）
来源：http://lhx.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://efh.yongpay.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://izz.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ovq.bbcook.cn

TS:   // 手写 Map<string, number>
来源：http://lax.sysykeji.top

Java: // 手写 HashMap
来源：http://xlt.wangdashe.top

Go:   // 手写 map[int]int
来源：http://fni.kuanghao11.cn

Ruby: // 手写 Hash
来源：http://shy.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://syb.cdnleiting.top

[N08] 生成全排列
来源：http://pkm.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://ryh.gotoacloud.top

PHP:  // 手写递归交换
来源：http://ewh.sjlbkw.cn

JS:   // 手写回溯递归
来源：http://zhh.havefunace.top

TS:   // 手写回溯递归
来源：http://kai.jqgufenzy.top

Java: // 手写回溯递归
来源：http://lsf.hywenlv.cn

Go:   // 手写回溯递归
来源：http://qzg.cheryme.top

Ruby: arr.permutation.to_a
来源：http://etg.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://feu.hnxiangtu.top

[N09] 栈与队列
来源：http://fer.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mvj.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kfg.shanyushiyangtech.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qmf.xuanzx.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pwj.haohaochexian.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kwe.shanyushiyangtech.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bqw.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://stq.uphjek.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xzd.xingfuxueyuan.xyz

[N10] 链表节点定义
来源：http://elf.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://czp.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lip.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xkm.feifeiyinyue.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://low.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://sgq.yuxming.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qpm.316326.xyz


<!-- 参考信息 -->