代发 wailian999

================================================================================
来源：http://fvr.yonumen.top

K. JSON 与序列化
来源：http://ngl.hcnkem.com

================================================================================
来源：http://yhp.yanxiufei.cn

[K01] 对象转 JSON 字符串
来源：http://cqh.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mgs.jqgufenzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ffv.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://zmy.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://csx.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://osb.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://iro.dianchejie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qtr.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ohe.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://mjd.shanyushiyangtech.top

Py:   json.loads(s)
来源：http://bbg.shanyushiyangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ftq.nanxinkj.top

JS:   JSON.parse(s)
来源：http://wxk.xuetiantiany.cn

TS:   JSON.parse(s)
来源：http://fvq.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fpu.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://tbi.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://rlp.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zzb.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://svt.sysykeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bnt.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rse.chenlongwang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tqy.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://uhk.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rmu.zhongyouzk.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qcb.xuanzx.com

Ruby: JSON.pretty_generate(obj)
来源：http://mbn.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ita.xuanzx.com

[K04] 读取 JSON 文件
来源：http://wqc.daria6918.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bwd.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://npx.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uve.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://grk.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wju.xylfe.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mmb.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uqf.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wzs.uphjek.com

[K05] 深拷贝对象
来源：http://lxl.birdmap.top

Py:   copy.deepcopy(obj)
来源：http://xch.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://fys.sxryk.cn

JS:   structuredClone(obj)
来源：http://fvx.redwolf501.top

TS:   structuredClone(obj)
来源：http://rvc.xylfe.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eiz.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gpr.zhoulong.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xrz.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rbc.ydzc1.top

[K06] 解析 URL 查询串
来源：http://gup.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ulv.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qhi.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bbn.tanke756.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uhh.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://doq.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://abn.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hfc.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ops.guowangkeji.top

[K07] 进制转换
来源：http://tmg.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vuw.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tiq.daxiang520.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nmj.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://edt.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://smf.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nio.ehwqpu.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qvg.hywenlv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qvj.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://jiv.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://pzs.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rpg.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://kdp.yfazqb.com

TS:   v8.serialize(obj)        // Node
来源：http://irq.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aka.ctjpmb.com

Go:   encoding/gob
来源：http://due.cashguo.top

Ruby: Marshal.dump(obj)
来源：http://xdj.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hqq.aibaodan.cn

================================================================================
来源：http://pkn.xylfe.cn

L. 网络请求
来源：http://duk.hywenlv.cn

================================================================================
来源：http://odo.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://uhb.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://znz.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rpo.sysykeji.top

JS:   await fetch(url)
来源：http://jva.cashguo.top

TS:   await fetch(url)
来源：http://rtf.yuanzhike.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vmd.zdbjq.cn

Go:   resp, err := http.Get(url)
来源：http://vys.shuidangran.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cfv.52xcode.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://joa.yonumen.top

[L02] 发送 POST JSON
来源：http://xfy.c1oappe.top

Py:   requests.post(url, json={"a": 1})
来源：http://dmz.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ijp.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xas.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://him.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qee.yfazqb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cbh.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lmm.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wrf.chenzaomai.com

[L03] 设置自定义请求头
来源：http://vor.yj202588.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eub.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aoz.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qhj.xuanzx.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cux.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yhe.jlsjyb.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yht.cucudq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gbt.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ges.yuxming.cn

[L04] 设置超时
来源：http://muh.xinyue.icu

Py:   requests.get(url, timeout=5)
来源：http://utz.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dxl.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iyh.tarul.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wut.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pgn.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://byk.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xru.tian-w.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://she.hnqzz.top

[L05] 上传文件（multipart）
来源：http://jsz.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ahb.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lua.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://moj.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ywt.birdmap.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rso.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kto.sweek.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vqg.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rjw.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://xst.52xcode.cn

Py:   resp.json()
来源：http://jyv.hongshengwenyu.top

PHP:  json_decode($body, true);
来源：http://jzp.9152youxi.cn

JS:   await resp.json()
来源：http://pjm.hongshengwenyu.top

TS:   await resp.json()
来源：http://hku.fehbvm.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xyp.yangfankeji.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jrn.ppjwa.cn

Ruby: JSON.parse(resp.body)
来源：http://zol.guowangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cgy.yongpay.top

[L07] 处理 HTTP 状态码
来源：http://cex.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ejz.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://acp.sjlbkw.cn

JS:   resp.ok;  resp.status
来源：http://ofx.tarul.cn

TS:   resp.ok;  resp.status
来源：http://hqe.feifeiyinyue.top

Java: resp.statusCode()
来源：http://uwt.hammf.cn

Go:   resp.StatusCode
来源：http://qmg.xuanzx.com

Ruby: resp.code.to_i
来源：http://pza.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://sgl.jyoumei.cn

[L08] 并发请求多个地址
来源：http://byn.hywenlv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cqp.xuetiantiany.cn

PHP:  curl_multi_init() 系列
来源：http://tdc.sweek.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bxi.bbcook.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zuh.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dca.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zhq.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rfd.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://diz.shuidangran.top

================================================================================
来源：http://mgs.ivvv.top

M. 命令行 / 进程 / 环境
来源：http://qca.meibo888.top

================================================================================
来源：http://vkb.hywenlv.cn

[M01] 读取命令行参数
来源：http://lqg.c1oappe.top

Py:   sys.argv[1:]
来源：http://bzl.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://jvs.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://vzw.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://ihj.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://tds.dianchejie.cn

Go:   os.Args[1:]
来源：http://xkh.jiagoushi.top

Ruby: ARGV
来源：http://eae.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://nlc.52xcode.cn

[M02] 读取环境变量
来源：http://nlx.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://bsz.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ppm.shangyingyoupin.top

JS:   process.env.HOME
来源：http://pxs.ywan-chungtsiang.top

TS:   process.env.HOME
来源：http://oxk.jinqigufen.top

Java: System.getenv("HOME")
来源：http://iqi.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dyw.316326.xyz

Ruby: ENV["HOME"]
来源：http://hbm.cqqwz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lwz.cucudq.cn

[M03] 执行外部命令
来源：http://uhq.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kwz.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://obt.zhoulong.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://hjp.mhx1999.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jkh.jyoumei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mjk.tianlin.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://lnu.xziqi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hnz.feifeiyinyue.top

C#:   Process.Start("ls", "-l");
来源：http://vto.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://wij.bjfxy.top

Py:   os.getcwd()
来源：http://red.nanxinkj.top

PHP:  getcwd();
来源：http://bpe.zhijiandao.cn

JS:   process.cwd()
来源：http://dpj.sweek.top

TS:   process.cwd()
来源：http://isq.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://ezl.jinghuilouyu.cn

Go:   os.Getwd()
来源：http://xre.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://nec.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://cpm.jinghuilouyu.cn

[M05] 设置退出码
来源：http://tjh.316326.xyz

Py:   sys.exit(1)
来源：http://xsu.yvedp.cn

PHP:  exit(1);
来源：http://avt.sweek.top

JS:   process.exit(1)
来源：http://dbv.yanxiufei.cn

TS:   process.exit(1)
来源：http://ztb.tanke756.top

Java: System.exit(1)
来源：http://lbo.iojbl.cn

Go:   os.Exit(1)
来源：http://uwj.pengpengdd.cyou

Ruby: exit 1
来源：http://gac.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ean.gotoacloud.top

[M06] 向标准错误输出
来源：http://iio.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://ama.fanxiaobao.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ldb.tianlin.xyz

JS:   console.error("err")
来源：http://mer.zhiwuduotai.top

TS:   console.error("err")
来源：http://yzn.smart0.xyz

Java: System.err.println("err")
来源：http://hlz.zhixingplan.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uat.zhoulong.xyz

Ruby: warn "err"
来源：http://pdn.ywan-chungtsiang.top

C#:   Console.Error.WriteLine("err")
来源：http://qpa.gogol.net.cn

[M07] 判断是否为主入口
来源：http://imz.zhoulong.xyz

Py:   if __name__ == "__main__":
来源：http://vsc.tian-w.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ygs.zhongyouzk.top

JS:   require.main === module
来源：http://qfg.yj202588.top

TS:   require.main === module
来源：http://tgu.jqgufenzy.top

Java: public static void main(String[] args)
来源：http://mod.fengsongda.top

Go:   func main()
来源：http://xwu.316326.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://miw.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://wby.shangyingyoupin.top

[M08] 获取系统与运行时信息
来源：http://alh.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://ksn.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://lhb.fktsv.cn

JS:   process.platform;  process.version
来源：http://vum.sweek.top

TS:   process.platform;  process.version
来源：http://zje.fktsv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dui.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qkv.hysaishi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://izf.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zrx.meibo888.top

================================================================================
来源：http://ooa.yuxming.cn

N. 数据结构与算法
来源：http://lie.vehdjk.com

================================================================================
来源：http://nxa.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://xqx.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://btl.tianlin.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pph.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fjo.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lts.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://ynt.c1oappe.top

Go:   sort.SearchInts(arr, x)
来源：http://xnz.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://thl.jinghuilouyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cwa.hammf.cn

[N02] 排序（工程实践用内置实现）
来源：http://ide.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://fod.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vjm.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yqu.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xep.zhaomingkeji.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qwp.sweek.top

Go:   slices.Sort(arr)
来源：http://anv.jinghuilouyu.cn

Ruby: arr.sort
来源：http://hbj.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qhf.vqdsnc.cn

[N03] 快速排序（分治示例）
来源：http://lwa.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rxk.pycfn.com

PHP:  // 递归实现，或用 usort
来源：http://dgt.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rcq.tanke756.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zdn.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xrf.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rdb.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://awu.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://zab.nwbrower.top

[N04] 斐波那契数列
来源：http://vjv.ydjk.org.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zfl.nanxuanxn.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wbo.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eto.yfazqb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dun.gzhubu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://auc.tarul.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ogx.gaohongyu789.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wsg.mhx1999.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://svs.shzxlz.cn

[N05] 最大公约数
来源：http://xfg.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://nhz.yanxiufei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rpe.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nce.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ecl.jlsjyb.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zzj.zhiwuduotai.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qhv.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://nkm.mhx1999.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xiz.jinqigufen.top

[N06] 判断回文字符串
来源：http://ypp.xinyue.icu

Py:   s == s[::-1]
来源：http://sfy.yonumen.top

PHP:  $s === strrev($s);
来源：http://vof.jinqigfzy.top

JS:   s === [...s].reverse().join("")
来源：http://sio.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://evo.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kok.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://bug.ehwqpu.com

Ruby: s == s.reverse
来源：http://xex.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://dxv.ybcxt.top

[N07] 两数之和（返回下标）
来源：http://bce.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ftt.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jkm.sjlbkw.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vcq.vqdsnc.cn

TS:   // 手写 Map<string, number>
来源：http://cnd.dianchejie.cn

Java: // 手写 HashMap
来源：http://lks.pycfn.com

Go:   // 手写 map[int]int
来源：http://drc.uphjek.com

Ruby: // 手写 Hash
来源：http://hma.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://bov.wangshuangyany.cn

[N08] 生成全排列
来源：http://cnb.sweek.top

Py:   itertools.permutations(arr)
来源：http://zfn.gzhubu.top

PHP:  // 手写递归交换
来源：http://vqm.zhengqikj.top

JS:   // 手写回溯递归
来源：http://uwa.ybcxt.top

TS:   // 手写回溯递归
来源：http://snz.dianchejie.cn

Java: // 手写回溯递归
来源：http://asp.snrcjt.cn

Go:   // 手写回溯递归
来源：http://hqm.yfazqb.com

Ruby: arr.permutation.to_a
来源：http://qwl.cqqwz.cn

C#:   // 手写回溯递归
来源：http://gdq.quarkkingdee.top


<!-- 参考信息 -->