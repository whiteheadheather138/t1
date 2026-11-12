代发 wailian999

[K02] JSON 字符串转对象
来源：http://txi.mhx1999.top

Py:   json.loads(s)
来源：http://odn.9152youxi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zsv.daxiang520.top

JS:   JSON.parse(s)
来源：http://idk.sufxvd.cn

TS:   JSON.parse(s)
来源：http://kuw.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iqv.xuetiantiany.cn

Go:   json.Unmarshal(data, &v)
来源：http://nyu.yonumen.top

Ruby: JSON.parse(s)
来源：http://sim.cheryme.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zqt.havefunace.top

[K03] JSON 美化输出（带缩进）
来源：http://iot.0kj1m.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bud.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nvg.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://ezs.ctjpmb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://tfe.cucudq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zjf.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ccc.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://bjw.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ywa.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://wlr.sysykeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ult.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xwp.hywenlv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xme.mhx1999.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ekw.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://edy.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zjx.ehwqpu.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://jmz.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://boo.gotoacloud.top

[K05] 深拷贝对象
来源：http://vyz.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://esz.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://yah.zhixingplan.top

JS:   structuredClone(obj)
来源：http://dzb.nwbrower.top

TS:   structuredClone(obj)
来源：http://yop.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pdv.zdqjudy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sht.feifeiyinyue.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sjg.jqgfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ken.cheryme.top

[K06] 解析 URL 查询串
来源：http://qyh.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rid.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pwl.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cxz.ivvv.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bai.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vzg.shanyushiyangtech.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://aji.gotoacloud.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://enu.zhaomingkeji.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bya.yongpay.top

[K07] 进制转换
来源：http://noo.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ziz.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gum.snrcjt.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bgt.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ymt.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xri.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hps.pengpengdd.cyou

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hvf.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jve.nanxinkj.top

[K08] 二进制序列化（非 JSON）
来源：http://xqn.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://nnu.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wqh.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://uyh.fzhhl.top

TS:   v8.serialize(obj)        // Node
来源：http://nou.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wmd.sxryk.cn

Go:   encoding/gob
来源：http://zyg.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://omj.hfpthk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ccr.gzhubu.top

================================================================================
来源：http://knw.hesvh.cn

L. 网络请求
来源：http://mvj.0kj1m.cn

================================================================================
来源：http://hhk.cdnleiting.top

[L01] 发送 GET 请求
来源：http://adn.yfazqb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://grw.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hft.gogol.net.cn

JS:   await fetch(url)
来源：http://vbx.hywenlv.cn

TS:   await fetch(url)
来源：http://wle.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://azn.yangfankeji.com

Go:   resp, err := http.Get(url)
来源：http://yrf.nwbrower.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dlg.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ffn.snrcjt.cn

[L02] 发送 POST JSON
来源：http://dei.pengpengdd.cyou

Py:   requests.post(url, json={"a": 1})
来源：http://lsv.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hiy.cucudq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xpn.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iun.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fzd.jiagoushi.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sch.316326.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jyi.zhongyouzk.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wjw.nanxinkj.top

[L03] 设置自定义请求头
来源：http://hvn.meibo888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sro.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wxl.hcnkem.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gmi.fengsongda.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ihn.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ach.xingfuxueyuan.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ehh.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rnj.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zwz.hfpthk.cn

[L04] 设置超时
来源：http://eoy.zhaomingkeji.xyz

Py:   requests.get(url, timeout=5)
来源：http://clu.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://acr.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rqp.jinghuilouyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ygv.zhoulong.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hum.hnqzz.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yly.tianlin.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lxk.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cvc.xuanzx.com

[L05] 上传文件（multipart）
来源：http://kus.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lka.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fmz.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://srk.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gqe.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hrf.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ijs.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://axw.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mra.hcnkem.com

[L06] 解析响应为 JSON
来源：http://rke.ppjwa.cn

Py:   resp.json()
来源：http://nvy.tarul.cn

PHP:  json_decode($body, true);
来源：http://att.hnxiangtu.top

JS:   await resp.json()
来源：http://ksp.sysykeji.top

TS:   await resp.json()
来源：http://niu.jinghuilouyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bek.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://igb.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://cfn.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bgf.sweek.top

[L07] 处理 HTTP 状态码
来源：http://olz.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fmh.daria6918.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jzd.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://kym.pycfn.com

TS:   resp.ok;  resp.status
来源：http://fal.c1oappe.top

Java: resp.statusCode()
来源：http://jww.yongpay.top

Go:   resp.StatusCode
来源：http://plv.gogol.net.cn

Ruby: resp.code.to_i
来源：http://ngu.shanyushiyangtech.top

C#:   (int)resp.StatusCode
来源：http://nxs.hysaishi.cn

[L08] 并发请求多个地址
来源：http://kmu.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fmn.pengpengdd.cyou

PHP:  curl_multi_init() 系列
来源：http://itl.redwolf501.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ada.hfpthk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://njs.xziqi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qcv.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dmh.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xdi.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dxg.hcnkem.com

================================================================================
来源：http://dmo.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://ezw.yvedp.cn

================================================================================
来源：http://jsx.ybcxt.top

[M01] 读取命令行参数
来源：http://ebh.dashuyun.cn

Py:   sys.argv[1:]
来源：http://cbn.hammf.cn

PHP:  $argv;  $argc;
来源：http://lzh.gaohongyu789.top

JS:   process.argv.slice(2)
来源：http://oyp.c1oappe.top

TS:   process.argv.slice(2)
来源：http://vjl.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://rdb.hongshengwenyu.top

Go:   os.Args[1:]
来源：http://rdh.ivvv.top

Ruby: ARGV
来源：http://hnq.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://ivd.wangdashe.top

[M02] 读取环境变量
来源：http://teu.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://csw.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vkg.tianlin.xyz

JS:   process.env.HOME
来源：http://liq.meibo888.top

TS:   process.env.HOME
来源：http://yoo.svipenyu.cn

Java: System.getenv("HOME")
来源：http://lpy.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oir.yj20258.top

Ruby: ENV["HOME"]
来源：http://edy.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ekv.fengsongda.top

[M03] 执行外部命令
来源：http://peq.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ubl.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pal.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lds.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zxn.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xdy.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://iba.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://miv.ctjpmb.com

C#:   Process.Start("ls", "-l");
来源：http://rdx.yuxming.cn

[M04] 获取当前工作目录
来源：http://xle.tanke756.top

Py:   os.getcwd()
来源：http://bef.shuidangran.top

PHP:  getcwd();
来源：http://exf.xuanzx.com

JS:   process.cwd()
来源：http://lwl.havefunace.top

TS:   process.cwd()
来源：http://bor.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://ecf.smart0.xyz

Go:   os.Getwd()
来源：http://nbr.yuxming.cn

Ruby: Dir.pwd
来源：http://gta.chenzaomai.com

C#:   Directory.GetCurrentDirectory()
来源：http://xqs.jyoumei.cn

[M05] 设置退出码
来源：http://kip.ydjk.org.cn

Py:   sys.exit(1)
来源：http://qbc.yj20258.top

PHP:  exit(1);
来源：http://bub.shzxlz.cn

JS:   process.exit(1)
来源：http://krg.xylfe.cn

TS:   process.exit(1)
来源：http://nvi.hywenlv.cn

Java: System.exit(1)
来源：http://bzc.xziqi.cn

Go:   os.Exit(1)
来源：http://lda.birdmap.top

Ruby: exit 1
来源：http://qoa.zycfv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mpn.tanke756.top

[M06] 向标准错误输出
来源：http://pbs.yuanzhike.top

Py:   print("err", file=sys.stderr)
来源：http://zkr.guannengcc.top

PHP:  fwrite(STDERR, "err\n");
来源：http://okm.gzhubu.top

JS:   console.error("err")
来源：http://bdi.xylfe.cn

TS:   console.error("err")
来源：http://gec.snrcjt.cn

Java: System.err.println("err")
来源：http://idd.iojbl.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uxx.haohaochexian.top

Ruby: warn "err"
来源：http://ylo.yj20258.top

C#:   Console.Error.WriteLine("err")
来源：http://jgp.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://ust.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://nyg.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://txj.iojbl.cn

JS:   require.main === module
来源：http://lyr.fanxiaobao.xyz

TS:   require.main === module
来源：http://mhp.ybcxt.top

Java: public static void main(String[] args)
来源：http://zyw.hysaishi.cn

Go:   func main()
来源：http://uvq.zycfv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bdi.hcnkem.com

C#:   static void Main(string[] args)
来源：http://ixb.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://jvz.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://tuy.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://vwk.cucudq.cn

JS:   process.platform;  process.version
来源：http://bfe.cashguo.top

TS:   process.platform;  process.version
来源：http://xye.zhaomingkeji.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xpk.fengsongda.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hva.hongshengwenyu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://odf.yueranfly.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tbs.xinyue.icu

================================================================================
来源：http://dxo.9152youxi.cn

N. 数据结构与算法
来源：http://cvg.yonumen.top

================================================================================
来源：http://dwb.hcnkem.com

[N01] 二分查找（有序数组）
来源：http://iim.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://zui.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vas.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mpd.ydzc1.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fqt.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gdk.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://zqe.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hhn.quarkkingdee.top

C#:   Array.BinarySearch(arr, x)
来源：http://nfg.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://nes.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://qob.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://trp.xuetiantiany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://now.cucudq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nyw.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://too.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://cbi.xziqi.cn

Ruby: arr.sort
来源：http://lxm.dashuyun.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qua.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://vor.cdnleiting.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zae.yongpay.top

PHP:  // 递归实现，或用 usort
来源：http://gwg.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nua.daxiang520.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oyi.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nom.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fpf.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nzd.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://fpt.jiagoushi.top

[N04] 斐波那契数列
来源：http://ygp.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uux.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vbs.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gkm.ywan-chungtsiang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ehh.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gsa.yj20258888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mzd.cheryme.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hae.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kre.ydjk.org.cn

[N05] 最大公约数
来源：http://jbr.vehdjk.com

Py:   math.gcd(a, b)
来源：http://hyc.yongpay.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gcv.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vkw.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xda.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cvv.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dkb.cucudq.cn

Ruby: a.gcd(b)
来源：http://qhy.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://inl.sxryk.cn

[N06] 判断回文字符串
来源：http://msi.0kj1m.cn

Py:   s == s[::-1]
来源：http://ijg.ppjwa.cn

PHP:  $s === strrev($s);
来源：http://lns.ctjpmb.com

JS:   s === [...s].reverse().join("")
来源：http://kri.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://nde.yongpay.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qmu.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://reo.shuidangran.top

Ruby: s == s.reverse
来源：http://uzj.hammf.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ryz.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://kxi.feifeiyinyue.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://udb.yuanzhike.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yek.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dzc.sufxvd.cn

TS:   // 手写 Map<string, number>
来源：http://znp.xingfuxueyuan.xyz

Java: // 手写 HashMap
来源：http://ngm.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://ftv.andypj.xyz

Ruby: // 手写 Hash
来源：http://bdq.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://svc.zhiwuduotai.top

[N08] 生成全排列
来源：http://nwr.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://uyj.chenlongwang.top

PHP:  // 手写递归交换
来源：http://nrx.yangfankeji.com

JS:   // 手写回溯递归
来源：http://sdy.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://pbf.ywan-chungtsiang.top

Java: // 手写回溯递归
来源：http://uup.xuetiantiany.cn

Go:   // 手写回溯递归
来源：http://yvk.nwbrower.top

Ruby: arr.permutation.to_a
来源：http://egx.ctjpmb.com

C#:   // 手写回溯递归
来源：http://umh.kuanghao11.cn

[N09] 栈与队列
来源：http://ubu.ydjk.org.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pkl.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mnx.shanyushiyangtech.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rfu.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://chp.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xqu.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lzg.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jbk.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vll.shangyingyoupin.top

[N10] 链表节点定义
来源：http://sva.wangdashe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hui.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tuc.yongpay.top


<!-- 参考信息 -->