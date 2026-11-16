代发 wailian999

================================================================================
来源：http://qcl.yanxiufei.cn

K. JSON 与序列化
来源：http://pcr.wangshuangyany.cn

================================================================================
来源：http://egb.ydzc1.top

[K01] 对象转 JSON 字符串
来源：http://rvf.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yjd.zdqjudy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hvw.bbcook.cn

JS:   JSON.stringify(obj)
来源：http://jym.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://ken.jinqigufen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fjb.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://tsu.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nwi.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qii.andypj.xyz

[K02] JSON 字符串转对象
来源：http://qzm.wangshuangyany.cn

Py:   json.loads(s)
来源：http://gyc.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://buo.vehdjk.com

JS:   JSON.parse(s)
来源：http://fcq.cdnleiting.top

TS:   JSON.parse(s)
来源：http://qld.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qal.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://nlp.cheryme.top

Ruby: JSON.parse(s)
来源：http://xqf.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ter.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://jof.yongpay.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vgo.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bfe.ppjwa.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fqp.sjlbkw.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jup.sxryk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pkq.vqdsnc.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ulg.shanyushiyangtech.top

Ruby: JSON.pretty_generate(obj)
来源：http://gcu.hammf.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rnp.zhongyouzk.top

[K04] 读取 JSON 文件
来源：http://jht.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iiq.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sco.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ypi.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pds.c1oappe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wzc.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oyp.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://ylv.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ltb.kuanghao11.cn

[K05] 深拷贝对象
来源：http://jej.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://rze.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://byy.ivvv.top

JS:   structuredClone(obj)
来源：http://zld.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://mlk.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://auz.xylfe.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ytm.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vrk.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sjw.vqdsnc.cn

[K06] 解析 URL 查询串
来源：http://vzt.ivvv.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rnq.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wlq.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wmm.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oxk.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ujg.xziqi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mwk.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jvd.uphjek.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://usw.jinqigufen.top

[K07] 进制转换
来源：http://qja.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hzr.pycfn.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zib.zdbjq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bcm.guannengcc.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mcy.yuanzhike.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://chs.cashguo.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dju.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nbc.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gyi.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://ngi.redwolf501.top

Py:   pickle.dumps(obj)
来源：http://xjm.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hxe.chenlongwang.top

JS:   v8.serialize(obj)        // Node
来源：http://zhn.hongshengwenyu.top

TS:   v8.serialize(obj)        // Node
来源：http://cwt.zhixingplan.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fep.jlsjyb.cn

Go:   encoding/gob
来源：http://qfv.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://bix.kuanghao11.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zvr.haohaochexian.top

================================================================================
来源：http://yhj.redwolf501.top

L. 网络请求
来源：http://ugt.xingfuxueyuan.xyz

================================================================================
来源：http://ynr.havefunace.top

[L01] 发送 GET 请求
来源：http://rlh.birdmap.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mcw.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://haf.chenzaomai.com

JS:   await fetch(url)
来源：http://djz.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://cpk.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wme.xingfuxueyuan.xyz

Go:   resp, err := http.Get(url)
来源：http://mlp.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vav.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nia.tianlin.xyz

[L02] 发送 POST JSON
来源：http://zbs.vehdjk.com

Py:   requests.post(url, json={"a": 1})
来源：http://gmd.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fkf.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hqe.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wvm.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kmr.zdbjq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vdv.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sed.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jxb.xuanzx.com

[L03] 设置自定义请求头
来源：http://buu.sjlbkw.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gwx.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hbu.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mvq.ydjk.org.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lkx.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cik.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sgk.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vwe.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://txd.yangfankeji.com

[L04] 设置超时
来源：http://iqj.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://ekd.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://szw.ybcxt.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zzn.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kxu.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sbk.jianghu66.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ohc.iojbl.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wak.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tjm.sweek.top

[L05] 上传文件（multipart）
来源：http://vjv.xingfuxueyuan.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jbm.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mbo.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qtk.chenlongwang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ntk.hcnkem.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qws.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fyu.tianlin.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vix.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://onj.ivvv.top

[L06] 解析响应为 JSON
来源：http://wrx.nwbrower.top

Py:   resp.json()
来源：http://uor.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://hyu.ydzc1.top

JS:   await resp.json()
来源：http://jpr.sufxvd.cn

TS:   await resp.json()
来源：http://don.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mqo.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ofm.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://rfb.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ion.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://qnl.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zao.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lhu.zhongyouzk.top

JS:   resp.ok;  resp.status
来源：http://yqd.shangyingyoupin.top

TS:   resp.ok;  resp.status
来源：http://mjg.svipenyu.cn

Java: resp.statusCode()
来源：http://pft.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://pzp.ehwqpu.com

Ruby: resp.code.to_i
来源：http://uft.zhongyouzk.top

C#:   (int)resp.StatusCode
来源：http://zzt.shzxlz.cn

[L08] 并发请求多个地址
来源：http://apf.jinqigfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xvw.hnxiangtu.top

PHP:  curl_multi_init() 系列
来源：http://fco.aizwys.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jlp.jinqigufen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tbd.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uau.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tdf.jianghu66.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pic.quarkkingdee.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yox.uphjek.com

================================================================================
来源：http://xsr.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境
来源：http://gwo.yueranfly.top

================================================================================
来源：http://hcb.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://rxr.yuxming.cn

Py:   sys.argv[1:]
来源：http://ccn.jinqigfzy.top

PHP:  $argv;  $argc;
来源：http://glo.xinyue.icu

JS:   process.argv.slice(2)
来源：http://dcb.sxryk.cn

TS:   process.argv.slice(2)
来源：http://jji.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://jov.shangyingyoupin.top

Go:   os.Args[1:]
来源：http://bmm.wangdashe.top

Ruby: ARGV
来源：http://vgc.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://wpp.chenjidiqi.icu

[M02] 读取环境变量
来源：http://rqj.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://wru.sufxvd.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dex.wangdashe.top

JS:   process.env.HOME
来源：http://shp.bbcook.cn

TS:   process.env.HOME
来源：http://uoe.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://piz.jqgfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jex.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://qju.nwbrower.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gki.xuanzx.com

[M03] 执行外部命令
来源：http://mnt.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zos.chenzaomai.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rql.mhx1999.top

JS:   child_process.execSync("ls -l").toString()
来源：http://idd.chenlongwang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://sed.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dmo.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ygh.jiagoushi.top

Ruby: system("ls -l");  `ls -l`
来源：http://bei.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://tgm.ydjk.org.cn

[M04] 获取当前工作目录
来源：http://mdx.0kj1m.cn

Py:   os.getcwd()
来源：http://koe.cashguo.top

PHP:  getcwd();
来源：http://ylu.fzhhl.top

JS:   process.cwd()
来源：http://wmb.hfpthk.cn

TS:   process.cwd()
来源：http://eqe.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://ugy.jianghu66.top

Go:   os.Getwd()
来源：http://oxd.hcnkem.com

Ruby: Dir.pwd
来源：http://zvj.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://utc.mhx1999.top

[M05] 设置退出码
来源：http://qds.ybcxt.top

Py:   sys.exit(1)
来源：http://tup.fktsv.cn

PHP:  exit(1);
来源：http://ang.jinqigfzy.top

JS:   process.exit(1)
来源：http://pxs.jinghuilouyu.cn

TS:   process.exit(1)
来源：http://gfu.mhx1999.top

Java: System.exit(1)
来源：http://qpx.birdmap.top

Go:   os.Exit(1)
来源：http://yha.gogol.net.cn

Ruby: exit 1
来源：http://wcw.zhiwuduotai.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dlw.zhoulong.xyz

[M06] 向标准错误输出
来源：http://mgl.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://kog.haohaochexian.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yhl.meibo888.top

JS:   console.error("err")
来源：http://kaa.wangdashe.top

TS:   console.error("err")
来源：http://etw.xziqi.cn

Java: System.err.println("err")
来源：http://xtq.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dbn.dashuyun.cn

Ruby: warn "err"
来源：http://fnl.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://pgh.guannengcc.top

[M07] 判断是否为主入口
来源：http://ugf.yanxiufei.cn

Py:   if __name__ == "__main__":
来源：http://fqe.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yfe.shangyingyoupin.top

JS:   require.main === module
来源：http://axl.daxiang520.top

TS:   require.main === module
来源：http://omo.ywan-chungtsiang.top

Java: public static void main(String[] args)
来源：http://lge.zhoulong.xyz

Go:   func main()
来源：http://slk.hfpthk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ghx.hcnkem.com

C#:   static void Main(string[] args)
来源：http://lyp.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://gon.bbcook.cn

Py:   platform.system();  platform.python_version()
来源：http://krr.jinyuanbaomall.cn

PHP:  PHP_OS;  phpversion();
来源：http://hmq.aibaodan.cn

JS:   process.platform;  process.version
来源：http://lsz.andypj.xyz

TS:   process.platform;  process.version
来源：http://rcb.tanke756.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mst.shzxlz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://glw.jqgufenzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cld.jinqigufen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wia.cheryme.top

================================================================================
来源：http://ihe.sjlbkw.cn

N. 数据结构与算法
来源：http://ibt.jinyuanbaomall.cn

================================================================================
来源：http://jgu.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://nuy.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://enw.xingfuxueyuan.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kjw.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ltn.yuxming.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sup.jqgufenzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://vfw.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://epv.zhengqikj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ywt.cqqwz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gyp.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://vyk.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://bpq.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rre.jqgfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nsm.xingfuxueyuan.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://aac.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zfn.yvedp.cn

Go:   slices.Sort(arr)
来源：http://cna.9152youxi.cn

Ruby: arr.sort
来源：http://qzq.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rmg.hfpthk.cn

[N03] 快速排序（分治示例）
来源：http://bro.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ljy.daxiang520.top

PHP:  // 递归实现，或用 usort
来源：http://oor.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://thv.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ysd.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bok.fengsongda.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zyz.wangdashe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xwe.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vtf.0kj1m.cn

[N04] 斐波那契数列
来源：http://pxf.zhiwuduotai.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://icd.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tmq.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fqm.zdqjudy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://afn.mhx1999.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://awq.shanyushiyangtech.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iaj.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sga.svipenyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://atu.jqgufenzy.top

[N05] 最大公约数
来源：http://hty.yanxiufei.cn

Py:   math.gcd(a, b)
来源：http://vtl.bbcook.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gvp.yongpay.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://odl.tianlin.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://edw.jlsjyb.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://atk.yj202588.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jum.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://hmw.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://txn.cheryme.top

[N06] 判断回文字符串
来源：http://ebc.hfpthk.cn

Py:   s == s[::-1]
来源：http://xys.chenlongwang.top

PHP:  $s === strrev($s);
来源：http://rzq.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://tud.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://crr.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nhl.xinyue.icu

Go:   // 双指针从两端比较
来源：http://iju.xuetiantiany.cn

Ruby: s == s.reverse
来源：http://rlx.yuxming.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://som.jianghu66.top

[N07] 两数之和（返回下标）
来源：http://bqw.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xdm.yj202588.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fyn.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://lnw.shuidangran.top

TS:   // 手写 Map<string, number>
来源：http://dlz.ywan-chungtsiang.top

Java: // 手写 HashMap
来源：http://xjp.yfazqb.com

Go:   // 手写 map[int]int
来源：http://jdj.jiagoushi.top

Ruby: // 手写 Hash
来源：http://pat.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://kqo.tanke756.top

[N08] 生成全排列
来源：http://cdo.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://qma.shuidangran.top

PHP:  // 手写递归交换
来源：http://qgd.yuxming.cn

JS:   // 手写回溯递归
来源：http://pnk.yvedp.cn

TS:   // 手写回溯递归
来源：http://ond.chenjidiqi.icu

Java: // 手写回溯递归
来源：http://zye.zhiwuduotai.top

Go:   // 手写回溯递归
来源：http://aus.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://rek.c1oappe.top

C#:   // 手写回溯递归
来源：http://xsc.jiagoushi.top


<!-- 参考信息 -->