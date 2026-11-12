代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nga.chenjidiqi.icu

Go:   json.Marshal(obj)
来源：http://oks.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kty.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://avx.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://kvq.xuanzx.com

Py:   json.loads(s)
来源：http://zqp.hcnkem.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pis.chenlongwang.top

JS:   JSON.parse(s)
来源：http://erb.xylfe.cn

TS:   JSON.parse(s)
来源：http://qvt.andypj.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ewk.iojbl.cn

Go:   json.Unmarshal(data, &v)
来源：http://ese.cashguo.top

Ruby: JSON.parse(s)
来源：http://wms.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hya.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://bsp.haohaochexian.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xwf.aizwys.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://spu.vehdjk.com

JS:   JSON.stringify(obj, null, 2)
来源：http://qdo.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://tql.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uof.mhx1999.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gba.wangshuangyany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wtl.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mvw.hammf.cn

[K04] 读取 JSON 文件
来源：http://nha.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bvr.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cwh.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ffu.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vly.zycfv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mch.xylfe.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sch.yvedp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://exc.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lof.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://kfb.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://scs.snrcjt.cn

PHP:  unserialize(serialize($obj));
来源：http://jus.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://ptu.uphjek.com

TS:   structuredClone(obj)
来源：http://htp.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://amw.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://voh.gogol.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://una.jqgufenzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://isk.hnqzz.top

[K06] 解析 URL 查询串
来源：http://nvr.zhaomingkeji.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hyk.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lef.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jpx.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qtv.hysaishi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mps.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://brw.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dpi.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fla.hesvh.cn

[K07] 进制转换
来源：http://sjb.ywan-chungtsiang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gpe.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://llx.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wzn.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cms.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lnk.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fzc.pengpengdd.cyou

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://flk.haohaochexian.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pah.zdbjq.cn

[K08] 二进制序列化（非 JSON）
来源：http://ezb.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://spb.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fvb.ctjpmb.com

JS:   v8.serialize(obj)        // Node
来源：http://cqa.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://foz.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rzz.gzhubu.top

Go:   encoding/gob
来源：http://ume.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://rvq.guannengcc.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jyy.redwolf501.top

================================================================================
来源：http://myz.xylfe.cn

L. 网络请求
来源：http://kwj.yfazqb.com

================================================================================
来源：http://grh.vehdjk.com

[L01] 发送 GET 请求
来源：http://kqq.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rby.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://upp.ybcxt.top

JS:   await fetch(url)
来源：http://lxz.chenjidiqi.icu

TS:   await fetch(url)
来源：http://yuv.yueranfly.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://szu.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://vbt.chenjidiqi.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://meb.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mip.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://hpg.xinyue.icu

Py:   requests.post(url, json={"a": 1})
来源：http://ntg.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gnl.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nst.yonumen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rme.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://djy.feifeiyinyue.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://glj.meibo888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yoj.shzxlz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rji.ydjk.org.cn

[L03] 设置自定义请求头
来源：http://zfu.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lfn.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kub.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nvm.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jlz.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iuh.quarkkingdee.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qni.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eoq.zdbjq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vol.shuidangran.top

[L04] 设置超时
来源：http://zbc.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://nax.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ihz.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ply.tanke756.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qkw.nwbrower.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uxx.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qnw.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rwp.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mrl.aizwys.cn

[L05] 上传文件（multipart）
来源：http://xwa.aibaodan.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cyx.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jdk.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jpw.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rtl.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tdy.epnwcf.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://igt.jianghu66.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fjy.hnxiangtu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yuo.fktsv.cn

[L06] 解析响应为 JSON
来源：http://zxg.xinyue.icu

Py:   resp.json()
来源：http://eza.jinghuilouyu.cn

PHP:  json_decode($body, true);
来源：http://utv.wangshuangyany.cn

JS:   await resp.json()
来源：http://gar.tarul.cn

TS:   await resp.json()
来源：http://zab.svipenyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lyz.guannengcc.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lcw.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://cxm.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pdn.sufxvd.cn

[L07] 处理 HTTP 状态码
来源：http://txy.jlsjyb.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bix.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bgg.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://scs.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://ueb.yueranfly.top

Java: resp.statusCode()
来源：http://ztd.gaohongyu789.top

Go:   resp.StatusCode
来源：http://odo.ctjpmb.com

Ruby: resp.code.to_i
来源：http://snl.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://kpw.zdbjq.cn

[L08] 并发请求多个地址
来源：http://dxj.fehbvm.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zap.yuxming.cn

PHP:  curl_multi_init() 系列
来源：http://rft.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://khf.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wow.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zri.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kpp.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tlc.zycfv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wwo.fengsongda.top

================================================================================
来源：http://aah.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://yvw.nwbrower.top

================================================================================
来源：http://wjr.gzhubu.top

[M01] 读取命令行参数
来源：http://unb.chenlongwang.top

Py:   sys.argv[1:]
来源：http://rpn.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://uvd.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://biu.mhx1999.top

TS:   process.argv.slice(2)
来源：http://zdz.tarul.cn

Java: args 数组（main 方法参数）
来源：http://dvm.ctjpmb.com

Go:   os.Args[1:]
来源：http://xjp.chenjidiqi.icu

Ruby: ARGV
来源：http://vtl.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://aak.havefunace.top

[M02] 读取环境变量
来源：http://dnu.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://qky.zdqjudy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gzk.nanxinkj.top

JS:   process.env.HOME
来源：http://drn.mhx1999.top

TS:   process.env.HOME
来源：http://jjr.jqgfzy.top

Java: System.getenv("HOME")
来源：http://mvf.guowangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zjl.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://bjb.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aim.ywan-chungtsiang.top

[M03] 执行外部命令
来源：http://wgm.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lts.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qdk.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vwh.zhongyouzk.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dcu.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ucq.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://fyc.chenzaomai.com

Ruby: system("ls -l");  `ls -l`
来源：http://byy.sufxvd.cn

C#:   Process.Start("ls", "-l");
来源：http://wgs.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://qeh.jiagoushi.top

Py:   os.getcwd()
来源：http://gza.gaohongyu789.top

PHP:  getcwd();
来源：http://qve.yongpay.top

JS:   process.cwd()
来源：http://gtl.haohaochexian.top

TS:   process.cwd()
来源：http://rvt.gogol.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://uso.0kj1m.cn

Go:   os.Getwd()
来源：http://tqz.gzhubu.top

Ruby: Dir.pwd
来源：http://jya.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tod.hywenlv.cn

[M05] 设置退出码
来源：http://vbm.fanxiaobao.xyz

Py:   sys.exit(1)
来源：http://xdi.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://ope.ybcxt.top

JS:   process.exit(1)
来源：http://oyo.yangfankeji.com

TS:   process.exit(1)
来源：http://eya.bjfxy.top

Java: System.exit(1)
来源：http://bmu.yuxming.cn

Go:   os.Exit(1)
来源：http://erk.wangshuangyany.cn

Ruby: exit 1
来源：http://wgx.jinghuilouyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ydz.yueranfly.top

[M06] 向标准错误输出
来源：http://apv.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://qck.shuidangran.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vtj.hfpthk.cn

JS:   console.error("err")
来源：http://gnb.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://mrg.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://kvs.andypj.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://amt.meibo888.top

Ruby: warn "err"
来源：http://gih.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://skl.tanke756.top

[M07] 判断是否为主入口
来源：http://ltp.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://ykc.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zwg.meibo888.top

JS:   require.main === module
来源：http://hck.9152youxi.cn

TS:   require.main === module
来源：http://oku.yongpay.top

Java: public static void main(String[] args)
来源：http://vnm.sufxvd.cn

Go:   func main()
来源：http://ozi.fanxiaobao.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zgq.snrcjt.cn

C#:   static void Main(string[] args)
来源：http://smf.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://bzl.gogol.net.cn

Py:   platform.system();  platform.python_version()
来源：http://tei.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://the.aizwys.cn

JS:   process.platform;  process.version
来源：http://mnp.gogol.net.cn

TS:   process.platform;  process.version
来源：http://mxx.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gdh.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ozu.svipenyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nei.zhongyouzk.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://euq.sweek.top

================================================================================
来源：http://yqh.0kj1m.cn

N. 数据结构与算法
来源：http://bze.birdmap.top

================================================================================
来源：http://xxu.bjfxy.top

[N01] 二分查找（有序数组）
来源：http://kgz.ehwqpu.com

Py:   bisect.bisect_left(arr, x)
来源：http://rzb.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bsn.iojbl.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bhl.hesvh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qew.zhoulong.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://wuz.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://vtb.c1oappe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://erj.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://myw.nanxinkj.top

[N02] 排序（工程实践用内置实现）
来源：http://rui.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://gpf.fengsongda.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://trx.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ync.guowangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vsz.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rfz.hesvh.cn

Go:   slices.Sort(arr)
来源：http://pco.bjfxy.top

Ruby: arr.sort
来源：http://ana.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dnq.mhx1999.top

[N03] 快速排序（分治示例）
来源：http://chn.bjfxy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jzh.vehdjk.com

PHP:  // 递归实现，或用 usort
来源：http://wik.nanxinkj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fbx.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://trf.jianghu66.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cco.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pcr.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ibg.yongpay.top

C#:   // 手写递归，或 Array.Sort
来源：http://nyo.zycfv.cn

[N04] 斐波那契数列
来源：http://jwd.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cvp.shzxlz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://akj.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xph.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kig.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://odr.ydzc1.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eqq.yuanzhike.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://khw.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ddo.xuanzx.com

[N05] 最大公约数
来源：http://nma.gzhubu.top

Py:   math.gcd(a, b)
来源：http://zcn.daxiang520.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ycd.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mga.ydzc1.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mnh.ivvv.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tom.ppjwa.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ijp.guannengcc.top

Ruby: a.gcd(b)
来源：http://plm.xinyue.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lsr.gogol.net.cn

[N06] 判断回文字符串
来源：http://ywf.tian-w.cn

Py:   s == s[::-1]
来源：http://zqr.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://uzz.yangfankeji.com

JS:   s === [...s].reverse().join("")
来源：http://pox.yonumen.top

TS:   s === [...s].reverse().join("")
来源：http://tha.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://plw.chenjidiqi.icu

Go:   // 双指针从两端比较
来源：http://jzr.xziqi.cn

Ruby: s == s.reverse
来源：http://ykp.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ieg.yj20258888.top

[N07] 两数之和（返回下标）
来源：http://hrd.uphjek.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qlb.zhoulong.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qyt.fengsongda.top

JS:   // 手写 Map：map.set(v, i)
来源：http://eyg.svipenyu.cn

TS:   // 手写 Map<string, number>
来源：http://mec.hcnkem.com

Java: // 手写 HashMap
来源：http://mzg.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://puw.yuxming.cn

Ruby: // 手写 Hash
来源：http://uqh.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fod.shuidangran.top

[N08] 生成全排列
来源：http://oto.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://vcm.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://kkw.fengsongda.top

JS:   // 手写回溯递归
来源：http://ukh.wangdashe.top

TS:   // 手写回溯递归
来源：http://twg.hcnkem.com

Java: // 手写回溯递归
来源：http://wsw.nanxinkj.top

Go:   // 手写回溯递归
来源：http://cyn.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://mnc.ywan-chungtsiang.top

C#:   // 手写回溯递归
来源：http://jgw.dashuyun.cn

[N09] 栈与队列
来源：http://njx.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sjf.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qix.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://avw.316326.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wkb.jinqigfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://toq.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qoc.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wxg.xuetiantiany.cn


<!-- 参考信息 -->