代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vbq.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://rjd.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://jww.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yno.uphjek.com

[K02] JSON 字符串转对象
来源：http://dig.sysykeji.top

Py:   json.loads(s)
来源：http://tjf.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ltr.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://ahe.fanxiaobao.xyz

TS:   JSON.parse(s)
来源：http://wsa.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gnj.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://swz.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://xoq.meibo888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nal.zhoulong.xyz

[K03] JSON 美化输出（带缩进）
来源：http://bpu.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dgx.fengsongda.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fhb.jinqigfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fgl.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qji.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jpd.redwolf501.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yrt.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://ove.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hpn.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://eba.yj20258888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wtr.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ivv.ydjk.org.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zfr.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eyr.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nfs.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oqf.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://yhd.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vpy.epnwcf.com

[K05] 深拷贝对象
来源：http://hoo.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://cmo.yanxiufei.cn

PHP:  unserialize(serialize($obj));
来源：http://jqs.sxryk.cn

JS:   structuredClone(obj)
来源：http://rof.yuanzhike.top

TS:   structuredClone(obj)
来源：http://xdk.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wrs.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jsw.aizwys.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://leo.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jif.jinqigfzy.top

[K06] 解析 URL 查询串
来源：http://teg.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ayb.svipenyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://msw.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://trf.sjlbkw.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vho.zhoulong.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qll.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qam.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qvt.epnwcf.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dvz.chenjidiqi.icu

[K07] 进制转换
来源：http://tvx.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kyv.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vce.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bce.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gfy.iojbl.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qzq.cucudq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nlf.cdnleiting.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ccp.zdqjudy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lxo.jiagoushi.top

[K08] 二进制序列化（非 JSON）
来源：http://vql.daria6918.cn

Py:   pickle.dumps(obj)
来源：http://eno.yonumen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zea.shangyingyoupin.top

JS:   v8.serialize(obj)        // Node
来源：http://amh.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://jsj.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tch.ivvv.top

Go:   encoding/gob
来源：http://yum.zhongyouzk.top

Ruby: Marshal.dump(obj)
来源：http://eew.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rhp.c1oappe.top

================================================================================
来源：http://hfk.yuanzhike.top

L. 网络请求
来源：http://akr.shangyingyoupin.top

================================================================================
来源：http://hyd.jinqigufen.top

[L01] 发送 GET 请求
来源：http://dmf.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jxh.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hii.sjlbkw.cn

JS:   await fetch(url)
来源：http://sxx.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://ewf.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vkm.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://pzm.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bwa.jiagoushi.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qcz.chenzaomai.com

[L02] 发送 POST JSON
来源：http://kmo.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://off.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dqv.zhengqikj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jdm.yanxiufei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vbf.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://drw.uphjek.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gni.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bmr.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uxt.cashguo.top

[L03] 设置自定义请求头
来源：http://ogo.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dot.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hsn.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nri.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vxt.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zhk.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ywm.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://okb.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jna.vqdsnc.cn

[L04] 设置超时
来源：http://rvr.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://wpf.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fgh.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ciu.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ubu.jinyuanbaomall.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yeg.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yzt.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rlq.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jsl.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://cba.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qqb.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://goe.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://phh.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jno.hnxiangtu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mcw.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lus.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gho.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://htn.havefunace.top

[L06] 解析响应为 JSON
来源：http://vtm.cashguo.top

Py:   resp.json()
来源：http://wuh.snrcjt.cn

PHP:  json_decode($body, true);
来源：http://txq.nwbrower.top

JS:   await resp.json()
来源：http://soi.haohaochexian.top

TS:   await resp.json()
来源：http://meo.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gbt.shzxlz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://glx.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://sor.hcnkem.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dkc.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://ifa.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xhv.nanxinkj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fbi.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://zbl.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://sqp.gotoacloud.top

Java: resp.statusCode()
来源：http://riz.xuanzx.com

Go:   resp.StatusCode
来源：http://lbx.cashguo.top

Ruby: resp.code.to_i
来源：http://veq.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://poj.haohaochexian.top

[L08] 并发请求多个地址
来源：http://cdv.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zti.jinyuanbaomall.cn

PHP:  curl_multi_init() 系列
来源：http://jbq.vehdjk.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ieg.fehbvm.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wsx.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://enx.yonumen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pzo.hongshengwenyu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uzw.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vzi.tarul.cn

================================================================================
来源：http://yxh.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://kgb.xuanzx.com

================================================================================
来源：http://dfo.jqgufenzy.top

[M01] 读取命令行参数
来源：http://gba.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://ibn.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://fcn.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://str.sysykeji.top

TS:   process.argv.slice(2)
来源：http://fye.yj202588.top

Java: args 数组（main 方法参数）
来源：http://pkd.jinqigufen.top

Go:   os.Args[1:]
来源：http://mgx.jyoumei.cn

Ruby: ARGV
来源：http://vdf.fengsongda.top

C#:   args 数组（Main 方法参数）
来源：http://mgh.52xcode.cn

[M02] 读取环境变量
来源：http://nrj.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://vid.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://unv.yuxming.cn

JS:   process.env.HOME
来源：http://jnv.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://thn.aibaodan.cn

Java: System.getenv("HOME")
来源：http://rbx.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lpw.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://bvq.wangshuangyany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://trv.bjfxy.top

[M03] 执行外部命令
来源：http://hcw.dashuyun.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rdf.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ams.yvedp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cdd.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qow.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fic.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://iip.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://cwb.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://hdv.aibaodan.cn

[M04] 获取当前工作目录
来源：http://amg.jyoumei.cn

Py:   os.getcwd()
来源：http://asc.shzxlz.cn

PHP:  getcwd();
来源：http://kts.yangfankeji.com

JS:   process.cwd()
来源：http://zbf.ivvv.top

TS:   process.cwd()
来源：http://ocx.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://cik.havefunace.top

Go:   os.Getwd()
来源：http://vtj.pengpengdd.cyou

Ruby: Dir.pwd
来源：http://rgj.zdbjq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wok.gzhubu.top

[M05] 设置退出码
来源：http://mjc.aizwys.cn

Py:   sys.exit(1)
来源：http://fja.jinqigufen.top

PHP:  exit(1);
来源：http://upb.hnxiangtu.top

JS:   process.exit(1)
来源：http://dzf.yongpay.top

TS:   process.exit(1)
来源：http://wsu.shzxlz.cn

Java: System.exit(1)
来源：http://cpu.smart0.xyz

Go:   os.Exit(1)
来源：http://sap.guowangkeji.top

Ruby: exit 1
来源：http://yjp.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://biy.cqqwz.cn

[M06] 向标准错误输出
来源：http://scv.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://xqh.kuanghao11.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ehc.zhiwuduotai.top

JS:   console.error("err")
来源：http://sry.hesvh.cn

TS:   console.error("err")
来源：http://tiy.tanke756.top

Java: System.err.println("err")
来源：http://lzf.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lyg.yuanzhike.top

Ruby: warn "err"
来源：http://wfj.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://yzp.cucudq.cn

[M07] 判断是否为主入口
来源：http://acj.yanxiufei.cn

Py:   if __name__ == "__main__":
来源：http://pjp.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sdh.pycfn.com

JS:   require.main === module
来源：http://txn.nwbrower.top

TS:   require.main === module
来源：http://cuw.ydzc1.top

Java: public static void main(String[] args)
来源：http://gqe.jinqigufen.top

Go:   func main()
来源：http://jru.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sfl.iojbl.cn

C#:   static void Main(string[] args)
来源：http://uoi.zhaomingkeji.xyz

[M08] 获取系统与运行时信息
来源：http://cnk.zhongyouzk.top

Py:   platform.system();  platform.python_version()
来源：http://rph.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://umj.jqgufenzy.top

JS:   process.platform;  process.version
来源：http://yho.chenlongwang.top

TS:   process.platform;  process.version
来源：http://tni.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xyh.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zeu.redwolf501.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://elm.nanxinkj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qby.sufxvd.cn

================================================================================
来源：http://afh.ywan-chungtsiang.top

N. 数据结构与算法
来源：http://qgh.yuanzhike.top

================================================================================
来源：http://tan.meibo888.top

[N01] 二分查找（有序数组）
来源：http://vlq.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tgd.epnwcf.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ruz.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nxi.jinqigfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zyx.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://str.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://tkh.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rlt.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://dam.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://rnk.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://pxk.zhongyouzk.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gci.cdnleiting.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cmk.ydzc1.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xym.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cyz.fehbvm.com

Go:   slices.Sort(arr)
来源：http://hpx.sweek.top

Ruby: arr.sort
来源：http://beq.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wru.cqqwz.cn

[N03] 快速排序（分治示例）
来源：http://jmd.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hhj.zycfv.cn

PHP:  // 递归实现，或用 usort
来源：http://bwq.jyoumei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pfn.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iwo.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gzx.hfpthk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sez.jinqigfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://efv.jqgfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://ekh.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://dny.xuanzx.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zlm.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bur.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://heh.feifeiyinyue.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qze.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ahr.sjlbkw.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vuk.wangdashe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://doh.jinqigfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cze.jqgufenzy.top

[N05] 最大公约数
来源：http://jpk.sweek.top

Py:   math.gcd(a, b)
来源：http://kzo.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pbk.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ycd.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rnz.shangyingyoupin.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zho.havefunace.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nef.52xcode.cn

Ruby: a.gcd(b)
来源：http://ewg.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sfr.andypj.xyz

[N06] 判断回文字符串
来源：http://tyx.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://ehf.ywan-chungtsiang.top

PHP:  $s === strrev($s);
来源：http://vnt.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://lgg.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://igg.sxryk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zzt.havefunace.top

Go:   // 双指针从两端比较
来源：http://orh.xingfuxueyuan.xyz

Ruby: s == s.reverse
来源：http://lfh.snrcjt.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://csl.hongshengwenyu.top

[N07] 两数之和（返回下标）
来源：http://psf.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uyb.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gje.jqgufenzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pry.hnqzz.top

TS:   // 手写 Map<string, number>
来源：http://enp.zhengqikj.top

Java: // 手写 HashMap
来源：http://ljn.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://xzo.9152youxi.cn

Ruby: // 手写 Hash
来源：http://tzv.zhoulong.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://gqy.fengsongda.top

[N08] 生成全排列
来源：http://eag.ivvv.top

Py:   itertools.permutations(arr)
来源：http://vff.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://dkp.redwolf501.top

JS:   // 手写回溯递归
来源：http://brm.zycfv.cn

TS:   // 手写回溯递归
来源：http://wde.wangdashe.top

Java: // 手写回溯递归
来源：http://ekx.hnxiangtu.top

Go:   // 手写回溯递归
来源：http://auv.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://nzi.cdnleiting.top

C#:   // 手写回溯递归
来源：http://ugj.yuanzhike.top

[N09] 栈与队列
来源：http://ffh.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lae.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jdi.ehwqpu.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ahs.fzhhl.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kux.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zuq.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uqi.chenjidiqi.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cux.redwolf501.top


<!-- 参考信息 -->