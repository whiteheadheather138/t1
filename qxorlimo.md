代发 wailian999

[K02] JSON 字符串转对象
来源：http://drh.yvedp.cn

Py:   json.loads(s)
来源：http://nhv.snrcjt.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bic.aibaodan.cn

JS:   JSON.parse(s)
来源：http://lgf.fengsongda.top

TS:   JSON.parse(s)
来源：http://ylp.9152youxi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ffz.sjlbkw.cn

Go:   json.Unmarshal(data, &v)
来源：http://tzh.iojbl.cn

Ruby: JSON.parse(s)
来源：http://rou.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aqn.hywenlv.cn

[K03] JSON 美化输出（带缩进）
来源：http://rwe.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lpo.0kj1m.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://afr.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sxq.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jwf.xylfe.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cdp.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fsz.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://cwx.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kgc.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://dsu.hnxiangtu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ezw.iojbl.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://egj.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dir.tian-w.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xlw.jinqigfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ijn.snrcjt.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gtm.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gcu.uphjek.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pdj.gzhubu.top

[K05] 深拷贝对象
来源：http://ghr.jqgfzy.top

Py:   copy.deepcopy(obj)
来源：http://jed.hywenlv.cn

PHP:  unserialize(serialize($obj));
来源：http://yat.ybcxt.top

JS:   structuredClone(obj)
来源：http://exw.aizwys.cn

TS:   structuredClone(obj)
来源：http://rxi.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hoj.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zey.shanyushiyangtech.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ihi.nanxuanxn.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wgt.yonumen.top

[K06] 解析 URL 查询串
来源：http://gji.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dei.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bdc.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tva.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sgh.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ade.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://wpn.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cwn.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ivo.bjfxy.top

[K07] 进制转换
来源：http://rvw.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pzn.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ams.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tku.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nhn.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ugc.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://agr.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://efp.ctjpmb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://szf.tianlin.xyz

[K08] 二进制序列化（非 JSON）
来源：http://zwo.birdmap.top

Py:   pickle.dumps(obj)
来源：http://dmm.hfpthk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sfw.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://xqy.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://nih.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://til.cdnleiting.top

Go:   encoding/gob
来源：http://eyc.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://qxo.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wsf.shangyingyoupin.top

================================================================================
来源：http://faf.bbcook.cn

L. 网络请求
来源：http://nsq.vqdsnc.cn

================================================================================
来源：http://tof.zhaomingkeji.xyz

[L01] 发送 GET 请求
来源：http://ssh.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gus.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xfy.gaohongyu789.top

JS:   await fetch(url)
来源：http://ylf.meibo888.top

TS:   await fetch(url)
来源：http://mpu.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://scc.hfpthk.cn

Go:   resp, err := http.Get(url)
来源：http://bzz.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mfa.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ezn.xziqi.cn

[L02] 发送 POST JSON
来源：http://tcf.gzhubu.top

Py:   requests.post(url, json={"a": 1})
来源：http://vlv.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xha.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ypq.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cay.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sab.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://usm.ctjpmb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bta.xylfe.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sth.nanxinkj.top

[L03] 设置自定义请求头
来源：http://mru.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lkm.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wjq.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kyj.jianghu66.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dnw.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kvm.zdbjq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yxi.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vuy.chenzaomai.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yag.meibo888.top

[L04] 设置超时
来源：http://afy.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://idm.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pis.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yqn.redwolf501.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ros.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pyh.shangyingyoupin.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://imv.jinghuilouyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cya.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pvp.mhx1999.top

[L05] 上传文件（multipart）
来源：http://shv.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uax.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://skq.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://znp.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wrx.yonumen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uqp.shangyingyoupin.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yub.hnqzz.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://udx.shuidangran.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://njr.ydzc1.top

[L06] 解析响应为 JSON
来源：http://tdy.yj20258.top

Py:   resp.json()
来源：http://mju.svipenyu.cn

PHP:  json_decode($body, true);
来源：http://tat.birdmap.top

JS:   await resp.json()
来源：http://toa.andypj.xyz

TS:   await resp.json()
来源：http://slx.xuetiantiany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eds.nanxinkj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hms.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://tjc.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wvp.c1oappe.top

[L07] 处理 HTTP 状态码
来源：http://adx.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kxw.chenjidiqi.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oos.hcnkem.com

JS:   resp.ok;  resp.status
来源：http://nnb.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://adg.xylfe.cn

Java: resp.statusCode()
来源：http://egg.zhixingplan.top

Go:   resp.StatusCode
来源：http://sbe.9152youxi.cn

Ruby: resp.code.to_i
来源：http://xow.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://kao.gotoacloud.top

[L08] 并发请求多个地址
来源：http://hzt.daxiang520.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rvd.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://ufd.fanxiaobao.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xzy.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kzw.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wes.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vzc.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mdz.nanxinkj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uwa.quarkkingdee.top

================================================================================
来源：http://aes.pengpengdd.cyou

M. 命令行 / 进程 / 环境
来源：http://ivg.yvedp.cn

================================================================================
来源：http://zau.zhijiandao.cn

[M01] 读取命令行参数
来源：http://hgy.aizwys.cn

Py:   sys.argv[1:]
来源：http://tsl.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://ykj.sjlbkw.cn

JS:   process.argv.slice(2)
来源：http://ein.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://mln.xziqi.cn

Java: args 数组（main 方法参数）
来源：http://dne.xylfe.cn

Go:   os.Args[1:]
来源：http://ntl.nanxuanxn.top

Ruby: ARGV
来源：http://qak.wangshuangyany.cn

C#:   args 数组（Main 方法参数）
来源：http://qgi.cdnleiting.top

[M02] 读取环境变量
来源：http://elm.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://nsd.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ctd.feifeiyinyue.top

JS:   process.env.HOME
来源：http://wfz.havefunace.top

TS:   process.env.HOME
来源：http://xzt.fanxiaobao.xyz

Java: System.getenv("HOME")
来源：http://hdd.shangyingyoupin.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pve.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://vzo.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pno.ydjk.org.cn

[M03] 执行外部命令
来源：http://ivy.sjlbkw.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://txx.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wlb.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wyg.hysaishi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yqt.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://joh.vqdsnc.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nhr.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uid.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://odo.yuxming.cn

[M04] 获取当前工作目录
来源：http://dex.ctjpmb.com

Py:   os.getcwd()
来源：http://xwe.gzhubu.top

PHP:  getcwd();
来源：http://cmq.yfazqb.com

JS:   process.cwd()
来源：http://nkd.xziqi.cn

TS:   process.cwd()
来源：http://hyu.gotoacloud.top

Java: Path.of("").toAbsolutePath()
来源：http://xmg.zdbjq.cn

Go:   os.Getwd()
来源：http://wnd.hnxiangtu.top

Ruby: Dir.pwd
来源：http://unf.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://jwa.9152youxi.cn

[M05] 设置退出码
来源：http://rnm.zdbjq.cn

Py:   sys.exit(1)
来源：http://fbl.pengpengdd.cyou

PHP:  exit(1);
来源：http://qzn.shuidangran.top

JS:   process.exit(1)
来源：http://edd.jlsjyb.cn

TS:   process.exit(1)
来源：http://ovd.cashguo.top

Java: System.exit(1)
来源：http://gjd.hnqzz.top

Go:   os.Exit(1)
来源：http://vha.xuanzx.com

Ruby: exit 1
来源：http://kch.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://euh.snrcjt.cn

[M06] 向标准错误输出
来源：http://iyz.cqqwz.cn

Py:   print("err", file=sys.stderr)
来源：http://umg.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qzq.andypj.xyz

JS:   console.error("err")
来源：http://duo.ydzc1.top

TS:   console.error("err")
来源：http://kbw.tian-w.cn

Java: System.err.println("err")
来源：http://hjm.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mcl.ivvv.top

Ruby: warn "err"
来源：http://wqc.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://jhb.wangdashe.top

[M07] 判断是否为主入口
来源：http://yfp.cdnleiting.top

Py:   if __name__ == "__main__":
来源：http://xid.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vpe.zdqjudy.top

JS:   require.main === module
来源：http://qnm.fehbvm.com

TS:   require.main === module
来源：http://ivk.yuanzhike.top

Java: public static void main(String[] args)
来源：http://pad.ywan-chungtsiang.top

Go:   func main()
来源：http://msy.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nnk.hammf.cn

C#:   static void Main(string[] args)
来源：http://iqf.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://bxa.0kj1m.cn

Py:   platform.system();  platform.python_version()
来源：http://vhy.cashguo.top

PHP:  PHP_OS;  phpversion();
来源：http://tnp.zhengqikj.top

JS:   process.platform;  process.version
来源：http://kqo.gogol.net.cn

TS:   process.platform;  process.version
来源：http://qjf.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uts.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://vhu.epnwcf.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iga.sweek.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jpc.hammf.cn

================================================================================
来源：http://sxn.fanxiaobao.xyz

N. 数据结构与算法
来源：http://hhm.tanke756.top

================================================================================
来源：http://rjx.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://rxc.wangdashe.top

Py:   bisect.bisect_left(arr, x)
来源：http://bde.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xwm.zhixingplan.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kcy.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xzd.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hly.xingfuxueyuan.xyz

Go:   sort.SearchInts(arr, x)
来源：http://jqc.ctjpmb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://kdz.hesvh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wsr.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://hgv.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://gwi.jiagoushi.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ttv.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sjq.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wqg.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xxi.sweek.top

Go:   slices.Sort(arr)
来源：http://pbr.jlsjyb.cn

Ruby: arr.sort
来源：http://nlt.yonumen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://eic.fzhhl.top

[N03] 快速排序（分治示例）
来源：http://qbb.haohaochexian.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sia.shangyingyoupin.top

PHP:  // 递归实现，或用 usort
来源：http://pwq.zhengqikj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bfy.yfazqb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fkw.tianlin.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kbg.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oxq.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wlx.gotoacloud.top

C#:   // 手写递归，或 Array.Sort
来源：http://fuw.nanxuanxn.top

[N04] 斐波那契数列
来源：http://eeg.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pkn.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://irp.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hdg.cucudq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dng.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yqq.sysykeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hrg.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dqr.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oji.yanxiufei.cn

[N05] 最大公约数
来源：http://kua.tarul.cn

Py:   math.gcd(a, b)
来源：http://sqb.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ttb.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vkd.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aob.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://asg.yj20258.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fkw.shzxlz.cn

Ruby: a.gcd(b)
来源：http://vjt.kuanghao11.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://daq.ppjwa.cn

[N06] 判断回文字符串
来源：http://fyo.aizwys.cn

Py:   s == s[::-1]
来源：http://rmv.xuetiantiany.cn

PHP:  $s === strrev($s);
来源：http://lsz.shangyingyoupin.top

JS:   s === [...s].reverse().join("")
来源：http://uzx.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://vtj.sxryk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://esr.hammf.cn

Go:   // 双指针从两端比较
来源：http://paf.yfazqb.com

Ruby: s == s.reverse
来源：http://tqi.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xkm.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://qyp.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uxx.zdbjq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dif.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kwt.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://dne.9152youxi.cn

Java: // 手写 HashMap
来源：http://htc.redwolf501.top

Go:   // 手写 map[int]int
来源：http://iyv.kuanghao11.cn

Ruby: // 手写 Hash
来源：http://dar.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://azj.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://yjr.havefunace.top

Py:   itertools.permutations(arr)
来源：http://xao.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://cmz.jyoumei.cn

JS:   // 手写回溯递归
来源：http://zdg.daria6918.cn

TS:   // 手写回溯递归
来源：http://ofm.shanyushiyangtech.top

Java: // 手写回溯递归
来源：http://ovv.jianghu66.top

Go:   // 手写回溯递归
来源：http://hbf.zhaomingkeji.xyz

Ruby: arr.permutation.to_a
来源：http://yha.jianghu66.top

C#:   // 手写回溯递归
来源：http://qfa.hcnkem.com

[N09] 栈与队列
来源：http://fza.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lna.jianghu66.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mpp.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nor.zhixingplan.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gii.haohaochexian.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zwc.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yvj.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lut.zhijiandao.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tej.sufxvd.cn

[N10] 链表节点定义
来源：http://zex.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qub.ydjk.org.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bbu.guowangkeji.top


<!-- 参考信息 -->