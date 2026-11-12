代发 wailian999

[K02] JSON 字符串转对象
来源：http://fcq.316326.xyz

Py:   json.loads(s)
来源：http://zha.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iof.yonumen.top

JS:   JSON.parse(s)
来源：http://kuj.gotoacloud.top

TS:   JSON.parse(s)
来源：http://kdh.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qlf.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://inj.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://vua.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://unr.vqdsnc.cn

[K03] JSON 美化输出（带缩进）
来源：http://wng.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vvj.316326.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ghz.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kii.chenjidiqi.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://kqa.bbcook.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dic.redwolf501.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://edx.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ykv.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tat.xinyue.icu

[K04] 读取 JSON 文件
来源：http://spu.hesvh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ips.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lai.dianchejie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ivb.zhiwuduotai.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tww.jinghuilouyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qju.birdmap.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zad.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://owd.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rmn.yanxiufei.cn

[K05] 深拷贝对象
来源：http://kcs.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://nqo.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://wii.9152youxi.cn

JS:   structuredClone(obj)
来源：http://wjo.hysaishi.cn

TS:   structuredClone(obj)
来源：http://pas.ybcxt.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dii.bbcook.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mlh.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://epu.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://nsh.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://zih.jiagoushi.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://amc.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wcu.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://umu.gaohongyu789.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://frm.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lgj.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://smc.nwbrower.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lth.nanxinkj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tzd.cqqwz.cn

[K07] 进制转换
来源：http://dwt.jinqigfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zyy.jqgfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hge.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tld.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nmx.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://exc.jlsjyb.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ioo.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kbu.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xqs.shuidangran.top

[K08] 二进制序列化（非 JSON）
来源：http://kre.kuanghao11.cn

Py:   pickle.dumps(obj)
来源：http://igx.hongshengwenyu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wct.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://vvk.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://bay.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cvd.nanxinkj.top

Go:   encoding/gob
来源：http://dmk.shuidangran.top

Ruby: Marshal.dump(obj)
来源：http://vtr.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cov.gzhubu.top

================================================================================
来源：http://nev.havefunace.top

L. 网络请求
来源：http://pyp.jinghuilouyu.cn

================================================================================
来源：http://bma.redwolf501.top

[L01] 发送 GET 请求
来源：http://blc.yongpay.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bft.epnwcf.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://msa.yuxming.cn

JS:   await fetch(url)
来源：http://fsk.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://jqv.shzxlz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jnj.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://orb.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://txc.xuetiantiany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://voq.hfpthk.cn

[L02] 发送 POST JSON
来源：http://suy.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://gim.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://imi.9152youxi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qjf.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gdl.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bzf.zdqjudy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dyd.yj20258888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kwo.bjfxy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://usp.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://yhs.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kiz.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://msr.xinyue.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fvo.316326.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://igl.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mqj.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ewx.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yud.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pgz.zhoulong.xyz

[L04] 设置超时
来源：http://ygv.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://ynx.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://whi.52xcode.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gfr.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vxx.yfazqb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eak.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bqs.chenzaomai.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dfj.smart0.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://igm.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://tmh.wangdashe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://izx.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bmq.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://saj.yonumen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wnb.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://klb.nanxuanxn.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eat.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ddg.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gcc.ywan-chungtsiang.top

[L06] 解析响应为 JSON
来源：http://bdr.yvedp.cn

Py:   resp.json()
来源：http://uge.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://pno.yj20258.top

JS:   await resp.json()
来源：http://ydp.fanxiaobao.xyz

TS:   await resp.json()
来源：http://axe.guowangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://icn.nanxinkj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://buf.hnqzz.top

Ruby: JSON.parse(resp.body)
来源：http://bzl.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mtu.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://rjd.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ycw.fanxiaobao.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hvf.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://nmv.mhx1999.top

TS:   resp.ok;  resp.status
来源：http://zzu.tanke756.top

Java: resp.statusCode()
来源：http://qge.redwolf501.top

Go:   resp.StatusCode
来源：http://lzk.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://rbe.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://gih.epnwcf.com

[L08] 并发请求多个地址
来源：http://wyh.gotoacloud.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rzd.chenlongwang.top

PHP:  curl_multi_init() 系列
来源：http://qbp.jinyuanbaomall.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mdo.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pna.vqdsnc.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oul.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yxy.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ukt.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ddm.epnwcf.com

================================================================================
来源：http://uzl.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://dhh.yonumen.top

================================================================================
来源：http://lgh.52xcode.cn

[M01] 读取命令行参数
来源：http://cta.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://rqk.pycfn.com

PHP:  $argv;  $argc;
来源：http://kal.uphjek.com

JS:   process.argv.slice(2)
来源：http://ylw.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://xnd.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://yyx.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://mdw.epnwcf.com

Ruby: ARGV
来源：http://pra.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://yvo.dianchejie.cn

[M02] 读取环境变量
来源：http://aha.meibo888.top

Py:   os.environ.get("HOME")
来源：http://rku.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bit.andypj.xyz

JS:   process.env.HOME
来源：http://jdr.jiagoushi.top

TS:   process.env.HOME
来源：http://kay.sysykeji.top

Java: System.getenv("HOME")
来源：http://zup.cqqwz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ayi.sxryk.cn

Ruby: ENV["HOME"]
来源：http://qhm.zhengqikj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jej.dashuyun.cn

[M03] 执行外部命令
来源：http://qhe.xziqi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gvi.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dzg.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wot.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://eew.uphjek.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ybn.jinqigfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wbr.cdnleiting.top

Ruby: system("ls -l");  `ls -l`
来源：http://ghp.xziqi.cn

C#:   Process.Start("ls", "-l");
来源：http://vpx.smart0.xyz

[M04] 获取当前工作目录
来源：http://zpz.dashuyun.cn

Py:   os.getcwd()
来源：http://dxg.cucudq.cn

PHP:  getcwd();
来源：http://blx.cqqwz.cn

JS:   process.cwd()
来源：http://gzw.zhijiandao.cn

TS:   process.cwd()
来源：http://tzn.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://glx.meibo888.top

Go:   os.Getwd()
来源：http://yff.chenzaomai.com

Ruby: Dir.pwd
来源：http://bun.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://lso.daria6918.cn

[M05] 设置退出码
来源：http://hjy.yuxming.cn

Py:   sys.exit(1)
来源：http://vsm.daxiang520.top

PHP:  exit(1);
来源：http://fdv.xylfe.cn

JS:   process.exit(1)
来源：http://sjv.fzhhl.top

TS:   process.exit(1)
来源：http://ooy.ybcxt.top

Java: System.exit(1)
来源：http://ool.316326.xyz

Go:   os.Exit(1)
来源：http://pvv.zhongyouzk.top

Ruby: exit 1
来源：http://nha.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rqm.tanke756.top

[M06] 向标准错误输出
来源：http://vll.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://qcv.nanxinkj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://suq.bjfxy.top

JS:   console.error("err")
来源：http://vsg.tian-w.cn

TS:   console.error("err")
来源：http://los.cheryme.top

Java: System.err.println("err")
来源：http://tyl.xuetiantiany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cgj.aibaodan.cn

Ruby: warn "err"
来源：http://wkx.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://wuh.xuanzx.com

[M07] 判断是否为主入口
来源：http://gzo.meibo888.top

Py:   if __name__ == "__main__":
来源：http://qcs.shanyushiyangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tcg.yangfankeji.com

JS:   require.main === module
来源：http://heh.smart0.xyz

TS:   require.main === module
来源：http://izy.9152youxi.cn

Java: public static void main(String[] args)
来源：http://xmk.shanyushiyangkeji.top

Go:   func main()
来源：http://eja.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eiy.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://rrh.xuetiantiany.cn

[M08] 获取系统与运行时信息
来源：http://imk.fengsongda.top

Py:   platform.system();  platform.python_version()
来源：http://dym.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://ezd.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://egf.daxiang520.top

TS:   process.platform;  process.version
来源：http://oxo.quarkkingdee.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gwa.feifeiyinyue.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yro.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://per.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xsg.jlsjyb.cn

================================================================================
来源：http://wew.dianchejie.cn

N. 数据结构与算法
来源：http://don.bbcook.cn

================================================================================
来源：http://eio.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://pnw.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://raw.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eca.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mad.shuidangran.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sie.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ajs.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://hlr.snrcjt.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zaq.chenlongwang.top

C#:   Array.BinarySearch(arr, x)
来源：http://smm.yueranfly.top

[N02] 排序（工程实践用内置实现）
来源：http://cod.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://kpq.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gkm.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bum.shanyushiyangtech.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lau.cashguo.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zbf.daxiang520.top

Go:   slices.Sort(arr)
来源：http://mrn.fanxiaobao.xyz

Ruby: arr.sort
来源：http://jer.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://klk.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://fmi.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dqn.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://qtm.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lph.hammf.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pxk.dianchejie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vmf.jinqigfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hym.nanxinkj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ymj.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jjl.c1oappe.top

[N04] 斐波那契数列
来源：http://chn.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qhc.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xsu.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lja.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tdh.shanyushiyangtech.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wdp.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qcu.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nds.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wxr.jyoumei.cn

[N05] 最大公约数
来源：http://alv.bbcook.cn

Py:   math.gcd(a, b)
来源：http://dls.shzxlz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://esy.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bzd.yuxming.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nty.andypj.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nnf.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iqa.52xcode.cn

Ruby: a.gcd(b)
来源：http://fge.cqqwz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jka.sufxvd.cn

[N06] 判断回文字符串
来源：http://gwd.yanxiufei.cn

Py:   s == s[::-1]
来源：http://isa.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://gst.zhoulong.xyz

JS:   s === [...s].reverse().join("")
来源：http://eqf.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://pdg.sweek.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qzc.yj20258888.top

Go:   // 双指针从两端比较
来源：http://jco.chenzaomai.com

Ruby: s == s.reverse
来源：http://vgt.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://iye.jqgufenzy.top

[N07] 两数之和（返回下标）
来源：http://myr.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hpa.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fwy.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://iaq.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://nzx.nwbrower.top

Java: // 手写 HashMap
来源：http://gdm.smart0.xyz

Go:   // 手写 map[int]int
来源：http://ybl.dianchejie.cn

Ruby: // 手写 Hash
来源：http://vmp.ydzc1.top

C#:   // 手写 Dictionary<int, int>
来源：http://sde.andypj.xyz

[N08] 生成全排列
来源：http://iqa.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://fvs.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://mtp.xuetiantiany.cn

JS:   // 手写回溯递归
来源：http://piv.wangshuangyany.cn

TS:   // 手写回溯递归
来源：http://ioy.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://pxy.gotoacloud.top

Go:   // 手写回溯递归
来源：http://ibz.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://jhz.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://oqt.aizwys.cn

[N09] 栈与队列
来源：http://agj.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://otv.yonumen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lmr.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mik.svipenyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ahb.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dvk.jlsjyb.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hei.tanke756.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://emq.ivvv.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jlr.zycfv.cn

[N10] 链表节点定义
来源：http://tqw.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ynt.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://drl.hesvh.cn


<!-- 参考信息 -->