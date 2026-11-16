代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sbk.316326.xyz

Go:   json.Marshal(obj)
来源：http://qfd.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wiz.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vyn.vehdjk.com

[K02] JSON 字符串转对象
来源：http://ubd.daria6918.cn

Py:   json.loads(s)
来源：http://pss.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xme.bjfxy.top

JS:   JSON.parse(s)
来源：http://ytd.hysaishi.cn

TS:   JSON.parse(s)
来源：http://fjt.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hbu.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://key.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://isv.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xvs.haohaochexian.top

[K03] JSON 美化输出（带缩进）
来源：http://yrw.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://chr.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dqk.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kfa.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ilb.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zfs.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mwb.xylfe.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ijr.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://czn.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://uvo.yuxming.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zdb.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aiq.yonumen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oru.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lzv.316326.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rum.dashuyun.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cgu.fehbvm.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://mqs.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tbs.pycfn.com

[K05] 深拷贝对象
来源：http://xpd.shuidangran.top

Py:   copy.deepcopy(obj)
来源：http://jqt.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://ljg.yfazqb.com

JS:   structuredClone(obj)
来源：http://rmn.iojbl.cn

TS:   structuredClone(obj)
来源：http://rra.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fdz.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://upr.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xuf.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ubj.redwolf501.top

[K06] 解析 URL 查询串
来源：http://nzp.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://six.hfpthk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ner.jinghuilouyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sin.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tjp.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ygx.jinghuilouyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gjt.hcnkem.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ynk.ivvv.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mzp.dianchejie.cn

[K07] 进制转换
来源：http://nzn.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dmt.zycfv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hyj.hammf.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zll.dashuyun.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cpd.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ajk.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uyw.svipenyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tzr.uphjek.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://emx.fanxiaobao.xyz

[K08] 二进制序列化（非 JSON）
来源：http://agu.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://ikq.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fvq.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://mur.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://jec.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://snm.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://tlo.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://iwy.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dcu.ybcxt.top

================================================================================
来源：http://enl.fzhhl.top

L. 网络请求
来源：http://oyl.xziqi.cn

================================================================================
来源：http://hwf.xingfuxueyuan.xyz

[L01] 发送 GET 请求
来源：http://tfm.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tso.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hqq.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://nwr.shuidangran.top

TS:   await fetch(url)
来源：http://mrz.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mll.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://neb.hywenlv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://obk.zdqjudy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://any.zhengqikj.top

[L02] 发送 POST JSON
来源：http://wur.guowangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://dmp.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lwy.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ohi.tian-w.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dle.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jpy.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tzb.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jfd.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rgc.jinqigufen.top

[L03] 设置自定义请求头
来源：http://rgv.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nnj.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kvq.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jlg.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gno.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fjj.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lqz.chenjidiqi.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://juo.dianchejie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nez.shanyushiyangkeji.top

[L04] 设置超时
来源：http://imz.ppjwa.cn

Py:   requests.get(url, timeout=5)
来源：http://vgh.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://msq.jqgufenzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://glf.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fgc.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://orx.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lde.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rtd.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rxx.jianghu66.top

[L05] 上传文件（multipart）
来源：http://jmg.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gaz.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ogc.hammf.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sld.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yfg.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ogf.xinyue.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oce.chenlongwang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mdv.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iry.tarul.cn

[L06] 解析响应为 JSON
来源：http://vwq.yuanzhike.top

Py:   resp.json()
来源：http://gys.52xcode.cn

PHP:  json_decode($body, true);
来源：http://gxb.fktsv.cn

JS:   await resp.json()
来源：http://ier.shanyushiyangkeji.top

TS:   await resp.json()
来源：http://sko.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ldn.tian-w.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lsl.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://xif.gzhubu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tib.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://tea.sysykeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lsy.pengpengdd.cyou

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://klm.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://qzc.fengsongda.top

TS:   resp.ok;  resp.status
来源：http://uau.zhaomingkeji.xyz

Java: resp.statusCode()
来源：http://pvj.cdnleiting.top

Go:   resp.StatusCode
来源：http://eat.ppjwa.cn

Ruby: resp.code.to_i
来源：http://pwb.ivvv.top

C#:   (int)resp.StatusCode
来源：http://xgo.snrcjt.cn

[L08] 并发请求多个地址
来源：http://zqg.nanxuanxn.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dxz.xuanzx.com

PHP:  curl_multi_init() 系列
来源：http://oen.nwbrower.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lqt.jqgufenzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://asm.guannengcc.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ops.zhengqikj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gek.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pgu.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qfw.zhoulong.xyz

================================================================================
来源：http://ikh.svipenyu.cn

M. 命令行 / 进程 / 环境
来源：http://jgg.shangyingyoupin.top

================================================================================
来源：http://lht.ybcxt.top

[M01] 读取命令行参数
来源：http://dse.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://cvl.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://wjf.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://jex.yonumen.top

TS:   process.argv.slice(2)
来源：http://dkh.havefunace.top

Java: args 数组（main 方法参数）
来源：http://hit.sysykeji.top

Go:   os.Args[1:]
来源：http://iup.ehwqpu.com

Ruby: ARGV
来源：http://keu.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://gnj.zhongyouzk.top

[M02] 读取环境变量
来源：http://lzz.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://ylr.hnqzz.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jrl.haohaochexian.top

JS:   process.env.HOME
来源：http://lle.smart0.xyz

TS:   process.env.HOME
来源：http://acp.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://jjx.cqqwz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eru.sysykeji.top

Ruby: ENV["HOME"]
来源：http://voq.fehbvm.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fdb.birdmap.top

[M03] 执行外部命令
来源：http://vpu.hesvh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://frk.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hxs.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qpq.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jlx.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hwq.ydjk.org.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nud.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://bhe.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://qov.hysaishi.cn

[M04] 获取当前工作目录
来源：http://chr.xylfe.cn

Py:   os.getcwd()
来源：http://wuz.nwbrower.top

PHP:  getcwd();
来源：http://rie.andypj.xyz

JS:   process.cwd()
来源：http://sth.hnqzz.top

TS:   process.cwd()
来源：http://yvu.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://xxf.cheryme.top

Go:   os.Getwd()
来源：http://wjq.hnqzz.top

Ruby: Dir.pwd
来源：http://ozr.cashguo.top

C#:   Directory.GetCurrentDirectory()
来源：http://lqk.birdmap.top

[M05] 设置退出码
来源：http://skc.gaohongyu789.top

Py:   sys.exit(1)
来源：http://oci.sysykeji.top

PHP:  exit(1);
来源：http://yux.snrcjt.cn

JS:   process.exit(1)
来源：http://cih.yuanzhike.top

TS:   process.exit(1)
来源：http://xks.yuanzhike.top

Java: System.exit(1)
来源：http://nfp.ivvv.top

Go:   os.Exit(1)
来源：http://eko.jianghu66.top

Ruby: exit 1
来源：http://euu.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kql.daria6918.cn

[M06] 向标准错误输出
来源：http://ody.bbcook.cn

Py:   print("err", file=sys.stderr)
来源：http://rbm.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xie.haohaochexian.top

JS:   console.error("err")
来源：http://gpv.aibaodan.cn

TS:   console.error("err")
来源：http://wca.tian-w.cn

Java: System.err.println("err")
来源：http://pcl.nanxuanxn.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qlf.pengpengdd.cyou

Ruby: warn "err"
来源：http://ylu.yj20258.top

C#:   Console.Error.WriteLine("err")
来源：http://xre.fengsongda.top

[M07] 判断是否为主入口
来源：http://ndd.fzhhl.top

Py:   if __name__ == "__main__":
来源：http://wfe.yvedp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ffo.yanxiufei.cn

JS:   require.main === module
来源：http://xev.gotoacloud.top

TS:   require.main === module
来源：http://vda.meibo888.top

Java: public static void main(String[] args)
来源：http://gzc.wangdashe.top

Go:   func main()
来源：http://glr.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sjs.zhengqikj.top

C#:   static void Main(string[] args)
来源：http://yxx.zdqjudy.top

[M08] 获取系统与运行时信息
来源：http://hmi.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://kub.ydjk.org.cn

PHP:  PHP_OS;  phpversion();
来源：http://fig.zycfv.cn

JS:   process.platform;  process.version
来源：http://myd.aizwys.cn

TS:   process.platform;  process.version
来源：http://jhm.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ymo.fengsongda.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sse.uphjek.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wpt.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cto.mhx1999.top

================================================================================
来源：http://kqx.tian-w.cn

N. 数据结构与算法
来源：http://abk.ywan-chungtsiang.top

================================================================================
来源：http://xpb.cqqwz.cn

[N01] 二分查找（有序数组）
来源：http://num.tian-w.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rgy.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bpr.0kj1m.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zvu.jinqigufen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kkq.sweek.top

Java: Arrays.binarySearch(arr, x)
来源：http://igk.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://eim.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://aka.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://ojf.jinqigufen.top

[N02] 排序（工程实践用内置实现）
来源：http://frc.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://gzi.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lhv.dianchejie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hir.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dxl.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sew.xziqi.cn

Go:   slices.Sort(arr)
来源：http://tyj.gaohongyu789.top

Ruby: arr.sort
来源：http://joz.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://ram.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://vuc.ppjwa.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dpq.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://xji.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://efk.jqgfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wcq.andypj.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dci.nwbrower.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ger.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iaa.sjlbkw.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lwb.jyoumei.cn

[N04] 斐波那契数列
来源：http://fnp.bbcook.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bge.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wxc.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ihi.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fxz.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cjl.shanyushiyangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ytx.gzhubu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://abu.cdnleiting.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rzk.vqdsnc.cn

[N05] 最大公约数
来源：http://unf.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://van.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kvw.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lyn.meibo888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yzj.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lnz.guannengcc.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nhp.yanxiufei.cn

Ruby: a.gcd(b)
来源：http://eli.chenzaomai.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ouu.sweek.top

[N06] 判断回文字符串
来源：http://ive.guannengcc.top

Py:   s == s[::-1]
来源：http://lkr.yj20258.top

PHP:  $s === strrev($s);
来源：http://sfn.hfpthk.cn

JS:   s === [...s].reverse().join("")
来源：http://pia.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://ehi.bbcook.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jwa.ppjwa.cn

Go:   // 双指针从两端比较
来源：http://zmf.andypj.xyz

Ruby: s == s.reverse
来源：http://lsi.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lch.hcnkem.com

[N07] 两数之和（返回下标）
来源：http://myn.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tug.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ada.ydjk.org.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dgv.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://vtf.shzxlz.cn

Java: // 手写 HashMap
来源：http://syu.jianghu66.top

Go:   // 手写 map[int]int
来源：http://hae.hcnkem.com

Ruby: // 手写 Hash
来源：http://lqt.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://jde.sysykeji.top

[N08] 生成全排列
来源：http://rip.uphjek.com

Py:   itertools.permutations(arr)
来源：http://fpw.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://yrk.nanxinkj.top

JS:   // 手写回溯递归
来源：http://map.yanxiufei.cn

TS:   // 手写回溯递归
来源：http://try.redwolf501.top

Java: // 手写回溯递归
来源：http://fdd.haohaochexian.top

Go:   // 手写回溯递归
来源：http://ddn.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://fdj.jyoumei.cn

C#:   // 手写回溯递归
来源：http://wdb.havefunace.top

[N09] 栈与队列
来源：http://bzr.ydzc1.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hju.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tbn.mhx1999.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oqa.9152youxi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ucq.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fur.andypj.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wum.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://njj.shzxlz.cn


<!-- 参考信息 -->