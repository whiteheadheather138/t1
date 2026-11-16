代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ypb.havefunace.top

Go:   json.Marshal(obj)
来源：http://pho.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://ihb.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hjj.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://qsm.hnqzz.top

Py:   json.loads(s)
来源：http://lsr.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vzh.hesvh.cn

JS:   JSON.parse(s)
来源：http://jwe.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://nex.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mzx.hywenlv.cn

Go:   json.Unmarshal(data, &v)
来源：http://nvn.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://cdv.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fcn.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://yuh.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rfd.tianlin.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://glg.shanyushiyangtech.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bbs.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xwh.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xba.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wcs.hysaishi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sea.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dfh.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://fkx.meibo888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mwm.chenlongwang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gjo.shuidangran.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oko.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wyt.jinqigfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ktk.xziqi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dui.svipenyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://epz.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gqk.sjlbkw.cn

[K05] 深拷贝对象
来源：http://edx.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://gbe.yj20258.top

PHP:  unserialize(serialize($obj));
来源：http://ecl.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://mgv.shanyushiyangtech.top

TS:   structuredClone(obj)
来源：http://qch.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://rwi.yj202588.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://amf.xuanzx.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ejh.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vyo.dashuyun.cn

[K06] 解析 URL 查询串
来源：http://qtr.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qpx.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wjg.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uit.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yao.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tpu.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pdg.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://clc.gotoacloud.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://biv.cucudq.cn

[K07] 进制转换
来源：http://vvf.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pwd.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pru.xuanzx.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://huc.yuanzhike.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dsh.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qtv.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jsp.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pcr.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aam.hnqzz.top

[K08] 二进制序列化（非 JSON）
来源：http://zmh.uphjek.com

Py:   pickle.dumps(obj)
来源：http://wqq.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://igx.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://tcj.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://hrr.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yly.hammf.cn

Go:   encoding/gob
来源：http://hfq.gotoacloud.top

Ruby: Marshal.dump(obj)
来源：http://cvs.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kkd.zhixingplan.top

================================================================================
来源：http://aff.guowangkeji.top

L. 网络请求
来源：http://omd.zdqjudy.top

================================================================================
来源：http://hkb.vehdjk.com

[L01] 发送 GET 请求
来源：http://frw.shzxlz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xod.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://suv.mhx1999.top

JS:   await fetch(url)
来源：http://huj.fengsongda.top

TS:   await fetch(url)
来源：http://hqe.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://exm.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://std.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://gri.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sev.cheryme.top

[L02] 发送 POST JSON
来源：http://oai.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://mop.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pea.uphjek.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tpr.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dzg.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dww.jinghuilouyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iqd.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sga.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bbz.ydzc1.top

[L03] 设置自定义请求头
来源：http://zrc.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pky.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gqk.hcnkem.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cik.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tot.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xjd.jinghuilouyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://duz.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jcm.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sbe.vqdsnc.cn

[L04] 设置超时
来源：http://cau.svipenyu.cn

Py:   requests.get(url, timeout=5)
来源：http://wqz.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ors.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kkt.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mih.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gid.tian-w.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vxr.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dir.yuxming.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lyq.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://sqg.hysaishi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dhm.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jqx.316326.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pig.wangshuangyany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nov.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://awj.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lcz.epnwcf.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uhu.zhiwuduotai.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hox.cdnleiting.top

[L06] 解析响应为 JSON
来源：http://miq.zhaomingkeji.xyz

Py:   resp.json()
来源：http://ejz.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://xen.andypj.xyz

JS:   await resp.json()
来源：http://lvi.jqgufenzy.top

TS:   await resp.json()
来源：http://twn.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ikn.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jib.gzhubu.top

Ruby: JSON.parse(resp.body)
来源：http://eke.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://smh.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://klo.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uax.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jsl.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://dbk.shangyingyoupin.top

TS:   resp.ok;  resp.status
来源：http://izi.pycfn.com

Java: resp.statusCode()
来源：http://bjw.yj20258.top

Go:   resp.StatusCode
来源：http://ifx.hfpthk.cn

Ruby: resp.code.to_i
来源：http://vpi.aibaodan.cn

C#:   (int)resp.StatusCode
来源：http://ilz.ybcxt.top

[L08] 并发请求多个地址
来源：http://saa.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xli.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://beb.xuetiantiany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zsf.yanxiufei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uhh.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qnq.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iuy.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://spd.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://exv.fktsv.cn

================================================================================
来源：http://ipz.xuanzx.com

M. 命令行 / 进程 / 环境
来源：http://srd.sufxvd.cn

================================================================================
来源：http://dyz.nanxinkj.top

[M01] 读取命令行参数
来源：http://eqr.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://gab.iojbl.cn

PHP:  $argv;  $argc;
来源：http://qii.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://qwo.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://snt.yueranfly.top

Java: args 数组（main 方法参数）
来源：http://mpd.cheryme.top

Go:   os.Args[1:]
来源：http://frd.fanxiaobao.xyz

Ruby: ARGV
来源：http://xyc.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://iuk.chenjidiqi.icu

[M02] 读取环境变量
来源：http://fsc.zhijiandao.cn

Py:   os.environ.get("HOME")
来源：http://xpv.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mid.nanxinkj.top

JS:   process.env.HOME
来源：http://xym.snrcjt.cn

TS:   process.env.HOME
来源：http://zbm.aizwys.cn

Java: System.getenv("HOME")
来源：http://iot.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lyk.zdqjudy.top

Ruby: ENV["HOME"]
来源：http://hao.xinyue.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pdn.9152youxi.cn

[M03] 执行外部命令
来源：http://moe.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blv.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://agq.jinqigufen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bnw.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://dut.chenzaomai.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://edv.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yqa.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yjl.cqqwz.cn

C#:   Process.Start("ls", "-l");
来源：http://qfa.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://jbm.wangdashe.top

Py:   os.getcwd()
来源：http://acl.dashuyun.cn

PHP:  getcwd();
来源：http://poy.guowangkeji.top

JS:   process.cwd()
来源：http://jkv.chenlongwang.top

TS:   process.cwd()
来源：http://mik.yangfankeji.com

Java: Path.of("").toAbsolutePath()
来源：http://lda.jinqigfzy.top

Go:   os.Getwd()
来源：http://ste.jqgfzy.top

Ruby: Dir.pwd
来源：http://wnw.dashuyun.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dzp.wangshuangyany.cn

[M05] 设置退出码
来源：http://azb.vqdsnc.cn

Py:   sys.exit(1)
来源：http://jyt.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://zqv.ydzc1.top

JS:   process.exit(1)
来源：http://jji.chenlongwang.top

TS:   process.exit(1)
来源：http://odc.smart0.xyz

Java: System.exit(1)
来源：http://dyw.xingfuxueyuan.xyz

Go:   os.Exit(1)
来源：http://ztk.xinyue.icu

Ruby: exit 1
来源：http://nxu.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://frd.hongshengwenyu.top

[M06] 向标准错误输出
来源：http://qws.yongpay.top

Py:   print("err", file=sys.stderr)
来源：http://dlx.birdmap.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bit.gzhubu.top

JS:   console.error("err")
来源：http://nqh.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://xeu.cdnleiting.top

Java: System.err.println("err")
来源：http://erk.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xpw.yongpay.top

Ruby: warn "err"
来源：http://sdp.shanyushiyangtech.top

C#:   Console.Error.WriteLine("err")
来源：http://glb.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://mhc.havefunace.top

Py:   if __name__ == "__main__":
来源：http://swg.sxryk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dzh.sweek.top

JS:   require.main === module
来源：http://djs.9152youxi.cn

TS:   require.main === module
来源：http://lwq.hammf.cn

Java: public static void main(String[] args)
来源：http://emv.xuanzx.com

Go:   func main()
来源：http://zdj.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fev.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://mxn.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://mwh.zhaomingkeji.xyz

Py:   platform.system();  platform.python_version()
来源：http://vqg.fzhhl.top

PHP:  PHP_OS;  phpversion();
来源：http://sfb.iojbl.cn

JS:   process.platform;  process.version
来源：http://lzz.zdqjudy.top

TS:   process.platform;  process.version
来源：http://xbs.gogol.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kxs.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jcw.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gmb.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://asg.sufxvd.cn

================================================================================
来源：http://zyc.aizwys.cn

N. 数据结构与算法
来源：http://lxb.cucudq.cn

================================================================================
来源：http://qzy.sufxvd.cn

[N01] 二分查找（有序数组）
来源：http://hzt.ctjpmb.com

Py:   bisect.bisect_left(arr, x)
来源：http://kfl.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ahl.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mwf.nanxinkj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fup.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fsp.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://mmv.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zfk.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://vfc.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://lad.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://ptl.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vbf.ydzc1.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vma.zhoulong.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://apj.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ccq.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://yzp.haohaochexian.top

Ruby: arr.sort
来源：http://mht.zdbjq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nit.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://rbw.jyoumei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sxt.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://shu.hnxiangtu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jis.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hpg.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gqp.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://btj.feifeiyinyue.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fzc.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://rtt.cqqwz.cn

[N04] 斐波那契数列
来源：http://ibh.tian-w.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rod.9152youxi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://skc.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rrn.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fey.hnqzz.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zzk.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cea.zhijiandao.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uiu.yvedp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uig.redwolf501.top

[N05] 最大公约数
来源：http://ian.ybcxt.top

Py:   math.gcd(a, b)
来源：http://zfl.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://efr.52xcode.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jle.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fdn.yvedp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bfm.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hbp.cashguo.top

Ruby: a.gcd(b)
来源：http://tjl.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mcc.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://efb.feifeiyinyue.top

Py:   s == s[::-1]
来源：http://ctx.dianchejie.cn

PHP:  $s === strrev($s);
来源：http://scr.fengsongda.top

JS:   s === [...s].reverse().join("")
来源：http://ikh.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://che.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vmz.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://zee.yangfankeji.com

Ruby: s == s.reverse
来源：http://yfy.yongpay.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gse.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://qwi.zdbjq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xzs.xylfe.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rpy.pycfn.com

JS:   // 手写 Map：map.set(v, i)
来源：http://xnn.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://hcj.gogol.net.cn

Java: // 手写 HashMap
来源：http://urk.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://yzu.dashuyun.cn

Ruby: // 手写 Hash
来源：http://mca.zdqjudy.top

C#:   // 手写 Dictionary<int, int>
来源：http://peb.jiagoushi.top

[N08] 生成全排列
来源：http://dyc.zdbjq.cn

Py:   itertools.permutations(arr)
来源：http://umf.guowangkeji.top

PHP:  // 手写递归交换
来源：http://rjs.chenzaomai.com

JS:   // 手写回溯递归
来源：http://wuk.fengsongda.top

TS:   // 手写回溯递归
来源：http://ruz.zhengqikj.top

Java: // 手写回溯递归
来源：http://zmf.pengpengdd.cyou

Go:   // 手写回溯递归
来源：http://sdd.yfazqb.com

Ruby: arr.permutation.to_a
来源：http://pxp.jiagoushi.top

C#:   // 手写回溯递归
来源：http://qai.cheryme.top

[N09] 栈与队列
来源：http://bsv.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ekq.yonumen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uoz.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lsd.zhengqikj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zjk.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://efl.cashguo.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mip.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vwu.zhijiandao.cn


<!-- 参考信息 -->