代发 wailian999

================================================================================
来源：http://xuv.sxryk.cn

K. JSON 与序列化
来源：http://gtl.zhixingplan.top

================================================================================
来源：http://rft.epnwcf.com

[K01] 对象转 JSON 字符串
来源：http://pou.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bms.tianlin.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wtq.quarkkingdee.top

JS:   JSON.stringify(obj)
来源：http://rsw.feifeiyinyue.top

TS:   JSON.stringify(obj)
来源：http://hwd.bbcook.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wun.hammf.cn

Go:   json.Marshal(obj)
来源：http://sbr.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://lvc.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://evp.ivvv.top

[K02] JSON 字符串转对象
来源：http://dha.cqqwz.cn

Py:   json.loads(s)
来源：http://czk.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ebp.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://hjm.shanyushiyangtech.top

TS:   JSON.parse(s)
来源：http://iaj.jinqigufen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fij.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://boq.jianghu66.top

Ruby: JSON.parse(s)
来源：http://ikq.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kwn.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://bav.gzhubu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zrh.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fqk.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uft.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pil.chenlongwang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nmj.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tqz.shanyushiyangtech.top

Ruby: JSON.pretty_generate(obj)
来源：http://tkn.iojbl.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mhl.aibaodan.cn

[K04] 读取 JSON 文件
来源：http://oxv.shanyushiyangtech.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wky.xingfuxueyuan.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vwu.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://puf.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hde.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fiu.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jfk.birdmap.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ree.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cvh.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://syi.sysykeji.top

Py:   copy.deepcopy(obj)
来源：http://pyr.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://twn.ppjwa.cn

JS:   structuredClone(obj)
来源：http://ien.zdqjudy.top

TS:   structuredClone(obj)
来源：http://wqd.gotoacloud.top

Java: // 手写拷贝构造，或序列化往返
来源：http://adv.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dkk.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kli.yuanzhike.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hog.fengsongda.top

[K06] 解析 URL 查询串
来源：http://cfr.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gge.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dtd.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rgh.daria6918.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://obb.aibaodan.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uxe.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://abt.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nsd.hcnkem.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lnm.cheryme.top

[K07] 进制转换
来源：http://bgb.xingfuxueyuan.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lhr.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://glc.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ilr.meibo888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ips.xuanzx.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bzh.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://khu.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://utj.ctjpmb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iqb.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://ahj.yfazqb.com

Py:   pickle.dumps(obj)
来源：http://fzv.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://pel.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://fzh.316326.xyz

TS:   v8.serialize(obj)        // Node
来源：http://uod.ppjwa.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://etp.shanyushiyangkeji.top

Go:   encoding/gob
来源：http://rrg.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://twq.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cpe.hnqzz.top

================================================================================
来源：http://cxz.fanxiaobao.xyz

L. 网络请求
来源：http://vry.guowangkeji.top

================================================================================
来源：http://akr.ehwqpu.com

[L01] 发送 GET 请求
来源：http://iuj.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ist.nanxinkj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gtl.iojbl.cn

JS:   await fetch(url)
来源：http://eks.cdnleiting.top

TS:   await fetch(url)
来源：http://cid.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://brr.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://ywc.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pkn.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ers.fktsv.cn

[L02] 发送 POST JSON
来源：http://eml.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://pkm.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ris.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pue.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mkv.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aww.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bab.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uod.aibaodan.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://alf.zdbjq.cn

[L03] 设置自定义请求头
来源：http://aew.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://npa.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://izp.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zca.yongpay.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xcd.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kgc.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qsa.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://puc.shuidangran.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hkf.jianghu66.top

[L04] 设置超时
来源：http://bfi.jinghuilouyu.cn

Py:   requests.get(url, timeout=5)
来源：http://ayh.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rxk.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zrd.zhongyouzk.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://grz.zhoulong.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://esl.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://knz.yuanzhike.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gun.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hdx.fktsv.cn

[L05] 上传文件（multipart）
来源：http://pyw.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://agu.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pva.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://epk.jinyuanbaomall.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rdd.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jao.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xej.jlsjyb.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wta.zhiwuduotai.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pag.gogol.net.cn

[L06] 解析响应为 JSON
来源：http://vjo.shzxlz.cn

Py:   resp.json()
来源：http://etf.zhengqikj.top

PHP:  json_decode($body, true);
来源：http://nxr.dianchejie.cn

JS:   await resp.json()
来源：http://fqo.fehbvm.com

TS:   await resp.json()
来源：http://hvh.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jsx.shzxlz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xgd.jyoumei.cn

Ruby: JSON.parse(resp.body)
来源：http://zmz.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://scy.ywan-chungtsiang.top

[L07] 处理 HTTP 状态码
来源：http://ggu.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sba.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zqa.shangyingyoupin.top

JS:   resp.ok;  resp.status
来源：http://elx.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://gtm.tianlin.xyz

Java: resp.statusCode()
来源：http://uyf.shzxlz.cn

Go:   resp.StatusCode
来源：http://xss.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://mpw.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://klu.quarkkingdee.top

[L08] 并发请求多个地址
来源：http://mua.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://exp.iojbl.cn

PHP:  curl_multi_init() 系列
来源：http://ikv.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://diy.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fxq.meibo888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yoq.xuetiantiany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://koh.cqqwz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://urt.hnxiangtu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eyk.gaohongyu789.top

================================================================================
来源：http://mfl.pengpengdd.cyou

M. 命令行 / 进程 / 环境
来源：http://lnz.hnxiangtu.top

================================================================================
来源：http://edl.tian-w.cn

[M01] 读取命令行参数
来源：http://ihi.jyoumei.cn

Py:   sys.argv[1:]
来源：http://bmb.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://pgy.hesvh.cn

JS:   process.argv.slice(2)
来源：http://rfs.hcnkem.com

TS:   process.argv.slice(2)
来源：http://llq.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://kou.xziqi.cn

Go:   os.Args[1:]
来源：http://tut.hammf.cn

Ruby: ARGV
来源：http://uxr.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://vvm.tianlin.xyz

[M02] 读取环境变量
来源：http://aow.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://rkg.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yrw.hysaishi.cn

JS:   process.env.HOME
来源：http://lry.feifeiyinyue.top

TS:   process.env.HOME
来源：http://shp.nwbrower.top

Java: System.getenv("HOME")
来源：http://ors.vehdjk.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uwe.bjfxy.top

Ruby: ENV["HOME"]
来源：http://xyy.xuetiantiany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://udl.yangfankeji.com

[M03] 执行外部命令
来源：http://cdi.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vsf.wangdashe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rdj.gogol.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vrd.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jtc.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jrc.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zwq.zhijiandao.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dmx.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://quy.xziqi.cn

[M04] 获取当前工作目录
来源：http://syj.guannengcc.top

Py:   os.getcwd()
来源：http://kll.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://kvz.sufxvd.cn

JS:   process.cwd()
来源：http://sru.dianchejie.cn

TS:   process.cwd()
来源：http://yio.bbcook.cn

Java: Path.of("").toAbsolutePath()
来源：http://sdl.tarul.cn

Go:   os.Getwd()
来源：http://puh.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://qev.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://bwp.xuetiantiany.cn

[M05] 设置退出码
来源：http://jki.jlsjyb.cn

Py:   sys.exit(1)
来源：http://yqv.52xcode.cn

PHP:  exit(1);
来源：http://jxy.guannengcc.top

JS:   process.exit(1)
来源：http://ygv.cucudq.cn

TS:   process.exit(1)
来源：http://ggl.hysaishi.cn

Java: System.exit(1)
来源：http://sge.hnqzz.top

Go:   os.Exit(1)
来源：http://dtb.gaohongyu789.top

Ruby: exit 1
来源：http://emk.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mof.birdmap.top

[M06] 向标准错误输出
来源：http://mqk.snrcjt.cn

Py:   print("err", file=sys.stderr)
来源：http://hlf.yfazqb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://obu.zhiwuduotai.top

JS:   console.error("err")
来源：http://lny.9152youxi.cn

TS:   console.error("err")
来源：http://nzf.hywenlv.cn

Java: System.err.println("err")
来源：http://bpk.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fts.snrcjt.cn

Ruby: warn "err"
来源：http://ase.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://ojw.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://bbv.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://wim.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ykm.yanxiufei.cn

JS:   require.main === module
来源：http://taw.shanyushiyangkeji.top

TS:   require.main === module
来源：http://rpe.daria6918.cn

Java: public static void main(String[] args)
来源：http://tvp.gotoacloud.top

Go:   func main()
来源：http://ezi.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ban.yuxming.cn

C#:   static void Main(string[] args)
来源：http://oxu.hesvh.cn

[M08] 获取系统与运行时信息
来源：http://zxq.meibo888.top

Py:   platform.system();  platform.python_version()
来源：http://zme.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://qzu.uphjek.com

JS:   process.platform;  process.version
来源：http://jgo.c1oappe.top

TS:   process.platform;  process.version
来源：http://nhn.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ryg.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xof.sufxvd.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zlt.havefunace.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gus.svipenyu.cn

================================================================================
来源：http://khc.jlsjyb.cn

N. 数据结构与算法
来源：http://qbf.nanxinkj.top

================================================================================
来源：http://irl.jinyuanbaomall.cn

[N01] 二分查找（有序数组）
来源：http://xic.yongpay.top

Py:   bisect.bisect_left(arr, x)
来源：http://knk.yuanzhike.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dlh.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vpx.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sfp.hesvh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://odu.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://sbq.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yhs.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://any.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://mya.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://acu.c1oappe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nvn.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bml.ivvv.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tqn.nwbrower.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cft.mhx1999.top

Go:   slices.Sort(arr)
来源：http://nxu.vehdjk.com

Ruby: arr.sort
来源：http://ach.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ujn.tarul.cn

[N03] 快速排序（分治示例）
来源：http://fwl.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pmt.mhx1999.top

PHP:  // 递归实现，或用 usort
来源：http://lfq.tarul.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://moz.chenlongwang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tub.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nvx.birdmap.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xfk.dianchejie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cgn.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://xbc.52xcode.cn

[N04] 斐波那契数列
来源：http://uvm.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xay.jqgfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hob.vqdsnc.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tcu.hongshengwenyu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jvz.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pyt.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://obj.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bfh.hnqzz.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qhc.wangdashe.top

[N05] 最大公约数
来源：http://wgf.cheryme.top

Py:   math.gcd(a, b)
来源：http://doq.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nhi.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://khi.quarkkingdee.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mco.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bml.haohaochexian.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xbb.meibo888.top

Ruby: a.gcd(b)
来源：http://phx.shanyushiyangtech.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sgx.fehbvm.com

[N06] 判断回文字符串
来源：http://gfl.gzhubu.top

Py:   s == s[::-1]
来源：http://idc.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://xvd.jyoumei.cn

JS:   s === [...s].reverse().join("")
来源：http://yvu.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://ank.ehwqpu.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dqf.cheryme.top

Go:   // 双指针从两端比较
来源：http://czq.bjfxy.top

Ruby: s == s.reverse
来源：http://xbv.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sde.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://mwl.jqgufenzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rjj.hongshengwenyu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lej.yvedp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://owc.guannengcc.top

TS:   // 手写 Map<string, number>
来源：http://xzg.andypj.xyz

Java: // 手写 HashMap
来源：http://tob.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://kna.snrcjt.cn

Ruby: // 手写 Hash
来源：http://sjz.zhixingplan.top

C#:   // 手写 Dictionary<int, int>
来源：http://khn.9152youxi.cn

[N08] 生成全排列
来源：http://knh.yfazqb.com

Py:   itertools.permutations(arr)
来源：http://nwi.hammf.cn

PHP:  // 手写递归交换
来源：http://jyy.gogol.net.cn

JS:   // 手写回溯递归
来源：http://gih.0kj1m.cn

TS:   // 手写回溯递归
来源：http://kyr.aizwys.cn

Java: // 手写回溯递归
来源：http://zxm.gotoacloud.top

Go:   // 手写回溯递归
来源：http://sme.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://lxg.9152youxi.cn

C#:   // 手写回溯递归
来源：http://yex.sufxvd.cn


<!-- 参考信息 -->