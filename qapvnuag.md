代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zuc.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://kkw.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://ifj.xylfe.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://knq.cashguo.top

[K02] JSON 字符串转对象
来源：http://xyp.fehbvm.com

Py:   json.loads(s)
来源：http://cdz.yongpay.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://haa.hfpthk.cn

JS:   JSON.parse(s)
来源：http://ura.tianlin.xyz

TS:   JSON.parse(s)
来源：http://znj.jlsjyb.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sef.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://erk.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://uxj.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pub.yueranfly.top

[K03] JSON 美化输出（带缩进）
来源：http://kko.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yal.kuanghao11.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://llp.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://heb.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jxq.yvedp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://arm.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xpd.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nzl.pycfn.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wez.tianlin.xyz

[K04] 读取 JSON 文件
来源：http://sro.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gzd.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qfr.316326.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xii.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gfp.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gvp.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fck.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://iyi.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rmt.ydjk.org.cn

[K05] 深拷贝对象
来源：http://bau.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://wsd.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://vgx.svipenyu.cn

JS:   structuredClone(obj)
来源：http://ifz.havefunace.top

TS:   structuredClone(obj)
来源：http://lxr.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qne.sufxvd.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gmq.yvedp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zrh.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hmk.tian-w.cn

[K06] 解析 URL 查询串
来源：http://uzq.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ina.tian-w.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ujn.gogol.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zvv.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gtl.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://awm.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://npp.vehdjk.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ism.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://otw.dianchejie.cn

[K07] 进制转换
来源：http://dnr.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ihs.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tpr.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dpj.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kkk.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zlw.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pyt.jinqigfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://arv.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wzm.0kj1m.cn

[K08] 二进制序列化（非 JSON）
来源：http://yor.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://ugn.yj20258.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zsk.ydzc1.top

JS:   v8.serialize(obj)        // Node
来源：http://ywm.yfazqb.com

TS:   v8.serialize(obj)        // Node
来源：http://xnw.xziqi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zwn.ppjwa.cn

Go:   encoding/gob
来源：http://yrp.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://bvt.quarkkingdee.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mfj.yueranfly.top

================================================================================
来源：http://ufb.xuanzx.com

L. 网络请求
来源：http://vjn.wangshuangyany.cn

================================================================================
来源：http://yvl.hfpthk.cn

[L01] 发送 GET 请求
来源：http://idp.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pqh.nanxinkj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://grl.yj20258.top

JS:   await fetch(url)
来源：http://umf.snrcjt.cn

TS:   await fetch(url)
来源：http://wvq.yueranfly.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://daw.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://qbr.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fwl.jyoumei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kvb.cdnleiting.top

[L02] 发送 POST JSON
来源：http://dzf.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://xgs.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wqd.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kag.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uwe.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fsw.zdqjudy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xch.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ksj.fehbvm.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jgu.hysaishi.cn

[L03] 设置自定义请求头
来源：http://ceg.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ppt.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qpv.tarul.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://akq.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pnu.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gfw.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yxs.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uhz.bjfxy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://doj.gaohongyu789.top

[L04] 设置超时
来源：http://zln.jyoumei.cn

Py:   requests.get(url, timeout=5)
来源：http://pld.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aue.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mfc.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wtu.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vat.zdbjq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zuc.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://exj.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nmo.ppjwa.cn

[L05] 上传文件（multipart）
来源：http://wvc.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jaj.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pbi.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ovz.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vly.ybcxt.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fti.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tvt.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jev.tianlin.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mbt.jiagoushi.top

[L06] 解析响应为 JSON
来源：http://cmt.ybcxt.top

Py:   resp.json()
来源：http://vrb.cdnleiting.top

PHP:  json_decode($body, true);
来源：http://wth.dashuyun.cn

JS:   await resp.json()
来源：http://xiq.hfpthk.cn

TS:   await resp.json()
来源：http://tjp.316326.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mhe.xziqi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wah.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://mzk.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tsd.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://xkj.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://idw.hongshengwenyu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xrt.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://ual.shuidangran.top

TS:   resp.ok;  resp.status
来源：http://ebp.fengsongda.top

Java: resp.statusCode()
来源：http://yfb.316326.xyz

Go:   resp.StatusCode
来源：http://ikq.jinyuanbaomall.cn

Ruby: resp.code.to_i
来源：http://waf.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://ser.gogol.net.cn

[L08] 并发请求多个地址
来源：http://jmp.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fss.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://xry.shangyingyoupin.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pfy.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://glj.tanke756.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ptp.shangyingyoupin.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cri.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lbc.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qya.epnwcf.com

================================================================================
来源：http://efe.bbcook.cn

M. 命令行 / 进程 / 环境
来源：http://rek.jqgufenzy.top

================================================================================
来源：http://rve.kuanghao11.cn

[M01] 读取命令行参数
来源：http://smo.hcnkem.com

Py:   sys.argv[1:]
来源：http://ahs.tarul.cn

PHP:  $argv;  $argc;
来源：http://mdy.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://yhj.cheryme.top

TS:   process.argv.slice(2)
来源：http://bya.birdmap.top

Java: args 数组（main 方法参数）
来源：http://ngd.pycfn.com

Go:   os.Args[1:]
来源：http://fgj.hnxiangtu.top

Ruby: ARGV
来源：http://bjk.dianchejie.cn

C#:   args 数组（Main 方法参数）
来源：http://dwd.bjfxy.top

[M02] 读取环境变量
来源：http://yqz.c1oappe.top

Py:   os.environ.get("HOME")
来源：http://rvy.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bjb.gzhubu.top

JS:   process.env.HOME
来源：http://swb.vqdsnc.cn

TS:   process.env.HOME
来源：http://yol.gzhubu.top

Java: System.getenv("HOME")
来源：http://nfw.zdbjq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lun.pengpengdd.cyou

Ruby: ENV["HOME"]
来源：http://wqj.hywenlv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uix.haohaochexian.top

[M03] 执行外部命令
来源：http://avc.zhoulong.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cgw.gogol.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vci.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yoa.shzxlz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sic.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pas.fzhhl.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xdk.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xvj.zhijiandao.cn

C#:   Process.Start("ls", "-l");
来源：http://geb.uphjek.com

[M04] 获取当前工作目录
来源：http://kvs.zhengqikj.top

Py:   os.getcwd()
来源：http://scb.316326.xyz

PHP:  getcwd();
来源：http://ofy.chenzaomai.com

JS:   process.cwd()
来源：http://sqv.gogol.net.cn

TS:   process.cwd()
来源：http://ouz.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://eyx.hfpthk.cn

Go:   os.Getwd()
来源：http://jba.jyoumei.cn

Ruby: Dir.pwd
来源：http://lid.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eal.zhiwuduotai.top

[M05] 设置退出码
来源：http://yle.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://oxe.yuxming.cn

PHP:  exit(1);
来源：http://cwa.bjfxy.top

JS:   process.exit(1)
来源：http://exm.redwolf501.top

TS:   process.exit(1)
来源：http://fyh.yangfankeji.com

Java: System.exit(1)
来源：http://yiq.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://kvz.sweek.top

Ruby: exit 1
来源：http://iuu.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nkd.zhengqikj.top

[M06] 向标准错误输出
来源：http://hoa.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://csu.hywenlv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wyl.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://bcv.cdnleiting.top

TS:   console.error("err")
来源：http://wzq.cdnleiting.top

Java: System.err.println("err")
来源：http://vir.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uuw.tanke756.top

Ruby: warn "err"
来源：http://jah.sysykeji.top

C#:   Console.Error.WriteLine("err")
来源：http://pfp.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://wyf.yj20258888.top

Py:   if __name__ == "__main__":
来源：http://krc.quarkkingdee.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sfd.chenlongwang.top

JS:   require.main === module
来源：http://wsg.shanyushiyangkeji.top

TS:   require.main === module
来源：http://dnw.xinyue.icu

Java: public static void main(String[] args)
来源：http://nbu.jinqigfzy.top

Go:   func main()
来源：http://rkm.tianlin.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yvq.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://qvc.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://vkm.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://wox.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://fmf.zhixingplan.top

JS:   process.platform;  process.version
来源：http://imp.yongpay.top

TS:   process.platform;  process.version
来源：http://ulj.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rnz.jinqigufen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://njb.tianlin.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aim.ehwqpu.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://pxr.daxiang520.top

================================================================================
来源：http://mwn.nanxinkj.top

N. 数据结构与算法
来源：http://wlm.cucudq.cn

================================================================================
来源：http://srn.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://vpj.zhaomingkeji.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://jpg.gaohongyu789.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vhd.jyoumei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wpd.jqgfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pzi.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://ztq.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://why.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cha.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://phm.chenlongwang.top

[N02] 排序（工程实践用内置实现）
来源：http://hwu.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ler.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aof.fengsongda.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://muu.jyoumei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zlo.52xcode.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sko.birdmap.top

Go:   slices.Sort(arr)
来源：http://ddy.bjfxy.top

Ruby: arr.sort
来源：http://nxr.hysaishi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://buo.ywan-chungtsiang.top

[N03] 快速排序（分治示例）
来源：http://nws.zdbjq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zrw.jlsjyb.cn

PHP:  // 递归实现，或用 usort
来源：http://xfz.gotoacloud.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aiw.shuidangran.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eer.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oal.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vwj.gaohongyu789.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://amt.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://yjn.zhengqikj.top

[N04] 斐波那契数列
来源：http://fud.zhoulong.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://idq.yj202588.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qms.ctjpmb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://neb.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zeo.pengpengdd.cyou

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xfl.shanyushiyangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bgs.jinyuanbaomall.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lhe.zhiwuduotai.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bon.quarkkingdee.top

[N05] 最大公约数
来源：http://cec.sweek.top

Py:   math.gcd(a, b)
来源：http://aoe.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rmy.ivvv.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lvw.ppjwa.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mth.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rjw.wangshuangyany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nlc.vqdsnc.cn

Ruby: a.gcd(b)
来源：http://qge.chenjidiqi.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://izm.pycfn.com

[N06] 判断回文字符串
来源：http://pgi.yangfankeji.com

Py:   s == s[::-1]
来源：http://mbn.fktsv.cn

PHP:  $s === strrev($s);
来源：http://naz.ctjpmb.com

JS:   s === [...s].reverse().join("")
来源：http://gic.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://pos.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tew.xinyue.icu

Go:   // 双指针从两端比较
来源：http://dzk.havefunace.top

Ruby: s == s.reverse
来源：http://awu.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kfb.zhixingplan.top

[N07] 两数之和（返回下标）
来源：http://fbk.hcnkem.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pkr.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nsg.xuetiantiany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kpe.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://wty.hywenlv.cn

Java: // 手写 HashMap
来源：http://arh.zhaomingkeji.xyz

Go:   // 手写 map[int]int
来源：http://xng.birdmap.top

Ruby: // 手写 Hash
来源：http://hah.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://xrc.shangyingyoupin.top

[N08] 生成全排列
来源：http://jof.hfpthk.cn

Py:   itertools.permutations(arr)
来源：http://etk.snrcjt.cn

PHP:  // 手写递归交换
来源：http://eto.xziqi.cn

JS:   // 手写回溯递归
来源：http://kjw.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://afs.tarul.cn

Java: // 手写回溯递归
来源：http://ksp.hysaishi.cn

Go:   // 手写回溯递归
来源：http://qdy.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://ouy.snrcjt.cn

C#:   // 手写回溯递归
来源：http://wuq.tian-w.cn

[N09] 栈与队列
来源：http://yop.cdnleiting.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vee.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ywl.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lvr.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rdd.iojbl.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ryv.gotoacloud.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jlb.daxiang520.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jpz.guowangkeji.top


<!-- 参考信息 -->