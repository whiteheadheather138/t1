代发 wailian999

================================================================================
来源：http://lxp.feifeiyinyue.top

K. JSON 与序列化
来源：http://mea.shangyingyoupin.top

================================================================================
来源：http://ypy.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://mcx.yanxiufei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qat.jyoumei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://chf.hcnkem.com

JS:   JSON.stringify(obj)
来源：http://cxq.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://pbu.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wrl.ybcxt.top

Go:   json.Marshal(obj)
来源：http://ntr.fengsongda.top

Ruby: obj.to_json                                     // require "json"
来源：http://oin.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://iwt.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://kln.tanke756.top

Py:   json.loads(s)
来源：http://qei.hysaishi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zex.sufxvd.cn

JS:   JSON.parse(s)
来源：http://cnv.aibaodan.cn

TS:   JSON.parse(s)
来源：http://alg.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jui.jqgufenzy.top

Go:   json.Unmarshal(data, &v)
来源：http://kdg.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://zgd.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dhc.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://plq.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nla.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ess.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://owf.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rqt.hysaishi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://war.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dpv.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://sok.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jld.hnqzz.top

[K04] 读取 JSON 文件
来源：http://oaa.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kng.yfazqb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iui.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://klk.hnxiangtu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://slj.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zli.yuanzhike.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ydz.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://apr.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yku.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://ver.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://wtt.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://edb.hammf.cn

JS:   structuredClone(obj)
来源：http://uza.sxryk.cn

TS:   structuredClone(obj)
来源：http://xdd.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tfq.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://piw.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rob.yuanzhike.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dxr.meibo888.top

[K06] 解析 URL 查询串
来源：http://vcd.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lcl.tarul.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vkl.jqgufenzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ims.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fnv.zycfv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hbi.jiagoushi.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://twi.iojbl.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bzj.cashguo.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jlz.cdnleiting.top

[K07] 进制转换
来源：http://pyc.mhx1999.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pza.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gmr.hysaishi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aob.tian-w.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tmz.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jpc.daria6918.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zus.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kkl.tanke756.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eoo.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://vtv.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://ysb.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://wqz.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://mae.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://rly.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ody.zdbjq.cn

Go:   encoding/gob
来源：http://qpu.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://cnl.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wnw.fehbvm.com

================================================================================
来源：http://llo.hnqzz.top

L. 网络请求
来源：http://mrh.yonumen.top

================================================================================
来源：http://cjy.xinyue.icu

[L01] 发送 GET 请求
来源：http://bhy.fktsv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hrj.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tgu.dianchejie.cn

JS:   await fetch(url)
来源：http://tsf.zhiwuduotai.top

TS:   await fetch(url)
来源：http://jqm.hammf.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hki.ybcxt.top

Go:   resp, err := http.Get(url)
来源：http://rqh.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://znx.sysykeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xwf.hammf.cn

[L02] 发送 POST JSON
来源：http://iba.epnwcf.com

Py:   requests.post(url, json={"a": 1})
来源：http://wyv.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iby.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cfk.dashuyun.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hmd.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vzb.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zjl.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ffz.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kwf.hfpthk.cn

[L03] 设置自定义请求头
来源：http://puh.ehwqpu.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tso.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wsd.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://old.gotoacloud.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dsd.316326.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ldp.iojbl.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ygw.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vsg.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gaq.cucudq.cn

[L04] 设置超时
来源：http://mkj.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://lrr.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gun.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cxm.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hav.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://txw.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gia.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qej.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nad.fktsv.cn

[L05] 上传文件（multipart）
来源：http://juj.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fdj.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sek.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://shg.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kdv.sysykeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eje.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ydn.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iqp.yuxming.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://loq.52xcode.cn

[L06] 解析响应为 JSON
来源：http://igz.yuxming.cn

Py:   resp.json()
来源：http://xwj.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://xzy.shuidangran.top

JS:   await resp.json()
来源：http://ugr.nanxuanxn.top

TS:   await resp.json()
来源：http://rnm.daxiang520.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://omc.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oyl.cucudq.cn

Ruby: JSON.parse(resp.body)
来源：http://cul.yj202588.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://anl.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://jku.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jxt.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dnc.chenlongwang.top

JS:   resp.ok;  resp.status
来源：http://lru.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://qqx.haohaochexian.top

Java: resp.statusCode()
来源：http://gfz.tarul.cn

Go:   resp.StatusCode
来源：http://yub.iojbl.cn

Ruby: resp.code.to_i
来源：http://tfl.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://pdo.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://dee.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zmk.yvedp.cn

PHP:  curl_multi_init() 系列
来源：http://zge.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qda.daria6918.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ryn.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jmf.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iuf.zhoulong.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://evh.hnxiangtu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://buk.yueranfly.top

================================================================================
来源：http://cef.vehdjk.com

M. 命令行 / 进程 / 环境
来源：http://vep.bbcook.cn

================================================================================
来源：http://vje.nwbrower.top

[M01] 读取命令行参数
来源：http://ows.yanxiufei.cn

Py:   sys.argv[1:]
来源：http://pqq.chenlongwang.top

PHP:  $argv;  $argc;
来源：http://dzq.feifeiyinyue.top

JS:   process.argv.slice(2)
来源：http://eoi.hesvh.cn

TS:   process.argv.slice(2)
来源：http://omv.havefunace.top

Java: args 数组（main 方法参数）
来源：http://tod.snrcjt.cn

Go:   os.Args[1:]
来源：http://ryo.yj20258888.top

Ruby: ARGV
来源：http://xiq.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://tjs.xziqi.cn

[M02] 读取环境变量
来源：http://fqw.yj202588.top

Py:   os.environ.get("HOME")
来源：http://vgd.haohaochexian.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qwi.yj202588.top

JS:   process.env.HOME
来源：http://tli.hnxiangtu.top

TS:   process.env.HOME
来源：http://ewk.chenlongwang.top

Java: System.getenv("HOME")
来源：http://egg.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vkn.fktsv.cn

Ruby: ENV["HOME"]
来源：http://fgx.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wcr.zhengqikj.top

[M03] 执行外部命令
来源：http://kni.tanke756.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://keh.hysaishi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pfl.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://euv.zhongyouzk.top

TS:   child_process.execSync("ls -l").toString()
来源：http://atp.hongshengwenyu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bev.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qgw.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://deo.chenzaomai.com

C#:   Process.Start("ls", "-l");
来源：http://hcp.haohaochexian.top

[M04] 获取当前工作目录
来源：http://oxv.dashuyun.cn

Py:   os.getcwd()
来源：http://ase.cashguo.top

PHP:  getcwd();
来源：http://kup.wangshuangyany.cn

JS:   process.cwd()
来源：http://wjw.yanxiufei.cn

TS:   process.cwd()
来源：http://wzm.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://iug.zhijiandao.cn

Go:   os.Getwd()
来源：http://hyv.wangshuangyany.cn

Ruby: Dir.pwd
来源：http://tpb.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://dhz.jlsjyb.cn

[M05] 设置退出码
来源：http://rsp.yvedp.cn

Py:   sys.exit(1)
来源：http://oyy.jianghu66.top

PHP:  exit(1);
来源：http://lkf.zhaomingkeji.xyz

JS:   process.exit(1)
来源：http://xvp.ctjpmb.com

TS:   process.exit(1)
来源：http://xus.yj202588.top

Java: System.exit(1)
来源：http://glg.guannengcc.top

Go:   os.Exit(1)
来源：http://tos.hnxiangtu.top

Ruby: exit 1
来源：http://gpf.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rlc.jyoumei.cn

[M06] 向标准错误输出
来源：http://zwp.wangshuangyany.cn

Py:   print("err", file=sys.stderr)
来源：http://rrm.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ihn.yongpay.top

JS:   console.error("err")
来源：http://wym.hammf.cn

TS:   console.error("err")
来源：http://voi.zdbjq.cn

Java: System.err.println("err")
来源：http://fvx.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jko.hcnkem.com

Ruby: warn "err"
来源：http://umt.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://pec.smart0.xyz

[M07] 判断是否为主入口
来源：http://uxf.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://lxv.tanke756.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tre.ydjk.org.cn

JS:   require.main === module
来源：http://scn.shangyingyoupin.top

TS:   require.main === module
来源：http://zke.tianlin.xyz

Java: public static void main(String[] args)
来源：http://hob.andypj.xyz

Go:   func main()
来源：http://ylb.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xri.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://jqz.xuetiantiany.cn

[M08] 获取系统与运行时信息
来源：http://zba.yfazqb.com

Py:   platform.system();  platform.python_version()
来源：http://yrd.cqqwz.cn

PHP:  PHP_OS;  phpversion();
来源：http://tnb.jinqigufen.top

JS:   process.platform;  process.version
来源：http://rcy.svipenyu.cn

TS:   process.platform;  process.version
来源：http://jhh.bbcook.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fid.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yti.sufxvd.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lbo.zhijiandao.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oky.yongpay.top

================================================================================
来源：http://sbj.jianghu66.top

N. 数据结构与算法
来源：http://pmw.cashguo.top

================================================================================
来源：http://vwc.shuidangran.top

[N01] 二分查找（有序数组）
来源：http://dsy.yfazqb.com

Py:   bisect.bisect_left(arr, x)
来源：http://cpe.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kbp.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dhu.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ddn.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://eyf.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://uqv.xuetiantiany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hvv.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kxt.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://dux.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://bxi.epnwcf.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gpd.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://spo.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ddt.svipenyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zru.bjfxy.top

Go:   slices.Sort(arr)
来源：http://lfh.shuidangran.top

Ruby: arr.sort
来源：http://ffv.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://waz.tianlin.xyz

[N03] 快速排序（分治示例）
来源：http://llb.cucudq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vrx.tarul.cn

PHP:  // 递归实现，或用 usort
来源：http://lbs.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ccj.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://omb.jinyuanbaomall.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gmi.vehdjk.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lmi.jlsjyb.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dmj.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://lqr.havefunace.top

[N04] 斐波那契数列
来源：http://tyt.shzxlz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gpv.tanke756.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://psc.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://psu.dashuyun.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://txu.svipenyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dqc.hammf.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jkz.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jym.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://krv.uphjek.com

[N05] 最大公约数
来源：http://hvp.hywenlv.cn

Py:   math.gcd(a, b)
来源：http://pdh.aibaodan.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://huv.ivvv.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gnp.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mso.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wzy.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://amg.sysykeji.top

Ruby: a.gcd(b)
来源：http://cww.hcnkem.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vzp.dianchejie.cn

[N06] 判断回文字符串
来源：http://xfp.fengsongda.top

Py:   s == s[::-1]
来源：http://bxa.cheryme.top

PHP:  $s === strrev($s);
来源：http://cyq.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://dem.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://kzz.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qfz.nanxinkj.top

Go:   // 双指针从两端比较
来源：http://wqn.gzhubu.top

Ruby: s == s.reverse
来源：http://kvr.jinyuanbaomall.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zoo.zhongyouzk.top

[N07] 两数之和（返回下标）
来源：http://msb.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bea.ybcxt.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lpw.yfazqb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://thh.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://cni.havefunace.top

Java: // 手写 HashMap
来源：http://wxq.guannengcc.top

Go:   // 手写 map[int]int
来源：http://ecj.hcnkem.com

Ruby: // 手写 Hash
来源：http://ibz.ydjk.org.cn

C#:   // 手写 Dictionary<int, int>
来源：http://man.ydzc1.top

[N08] 生成全排列
来源：http://qag.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://muy.fengsongda.top

PHP:  // 手写递归交换
来源：http://eko.cqqwz.cn

JS:   // 手写回溯递归
来源：http://bzl.jqgufenzy.top

TS:   // 手写回溯递归
来源：http://nff.hywenlv.cn

Java: // 手写回溯递归
来源：http://odg.shuidangran.top

Go:   // 手写回溯递归
来源：http://fna.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://fhd.fzhhl.top

C#:   // 手写回溯递归
来源：http://rdp.yueranfly.top


<!-- 参考信息 -->