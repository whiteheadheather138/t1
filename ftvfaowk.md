代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bzs.9152youxi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cyj.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://qvx.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://ndq.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cyj.chenzaomai.com

Go:   json.Marshal(obj)
来源：http://pkq.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://jxu.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yri.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://iuh.52xcode.cn

Py:   json.loads(s)
来源：http://pfp.hnxiangtu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hgh.dianchejie.cn

JS:   JSON.parse(s)
来源：http://ssk.mhx1999.top

TS:   JSON.parse(s)
来源：http://esa.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cwi.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://ufm.bjfxy.top

Ruby: JSON.parse(s)
来源：http://tss.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zsw.jinqigfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://nqh.wangshuangyany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://igq.zhiwuduotai.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vir.pycfn.com

JS:   JSON.stringify(obj, null, 2)
来源：http://jvx.yuxming.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kxn.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pjm.hammf.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ptk.jlsjyb.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ywn.gzhubu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rss.zdbjq.cn

[K04] 读取 JSON 文件
来源：http://via.yuanzhike.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gjf.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zmf.jinyuanbaomall.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aih.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gmc.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xrd.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jzj.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://iwf.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://odi.svipenyu.cn

[K05] 深拷贝对象
来源：http://dqi.316326.xyz

Py:   copy.deepcopy(obj)
来源：http://euz.shangyingyoupin.top

PHP:  unserialize(serialize($obj));
来源：http://ylw.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://mzu.jyoumei.cn

TS:   structuredClone(obj)
来源：http://rqp.jiagoushi.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cwl.daxiang520.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wtk.zhiwuduotai.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yyr.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qxi.hnqzz.top

[K06] 解析 URL 查询串
来源：http://sbn.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tdr.dianchejie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://edm.yonumen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rib.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tij.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pcr.shangyingyoupin.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qrz.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wze.wangshuangyany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qqt.chenlongwang.top

[K07] 进制转换
来源：http://ndh.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qvq.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lur.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iux.zhengqikj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://llt.jianghu66.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nuf.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nfj.guannengcc.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uun.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zgm.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://stx.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://ozy.gogol.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ugz.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://xpa.ctjpmb.com

TS:   v8.serialize(obj)        // Node
来源：http://rdm.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://scd.chenjidiqi.icu

Go:   encoding/gob
来源：http://blm.cashguo.top

Ruby: Marshal.dump(obj)
来源：http://gny.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vup.yuxming.cn

================================================================================
来源：http://hkb.jlsjyb.cn

L. 网络请求
来源：http://pli.cqqwz.cn

================================================================================
来源：http://iwj.yj20258.top

[L01] 发送 GET 请求
来源：http://ply.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ufb.jiagoushi.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rng.cdnleiting.top

JS:   await fetch(url)
来源：http://akl.sweek.top

TS:   await fetch(url)
来源：http://aqj.zhoulong.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fro.dashuyun.cn

Go:   resp, err := http.Get(url)
来源：http://ppz.ydjk.org.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kqw.chenjidiqi.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nxs.yfazqb.com

[L02] 发送 POST JSON
来源：http://hja.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://csi.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tgu.yuxming.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ykn.jinyuanbaomall.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wry.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gmv.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sac.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kxd.jyoumei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dfp.jinqigufen.top

[L03] 设置自定义请求头
来源：http://mzy.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kjk.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gvo.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oin.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xzj.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://snt.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kal.aibaodan.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fef.hnqzz.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://osb.shangyingyoupin.top

[L04] 设置超时
来源：http://wez.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://kfx.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bzb.hesvh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gyd.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tbo.gogol.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://giu.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jps.shanyushiyangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ldu.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eju.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://xag.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xid.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lbm.yj20258888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yau.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ikt.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://chp.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://axm.ywan-chungtsiang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vgm.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hyx.shangyingyoupin.top

[L06] 解析响应为 JSON
来源：http://fsr.zhengqikj.top

Py:   resp.json()
来源：http://ixy.sysykeji.top

PHP:  json_decode($body, true);
来源：http://rxu.wangdashe.top

JS:   await resp.json()
来源：http://noi.sufxvd.cn

TS:   await resp.json()
来源：http://yac.aibaodan.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lyy.cheryme.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://buz.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://asi.dianchejie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hlu.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://sdw.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rjt.aizwys.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qqu.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://caj.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://oij.iojbl.cn

Java: resp.statusCode()
来源：http://fzq.bjfxy.top

Go:   resp.StatusCode
来源：http://sdp.hnqzz.top

Ruby: resp.code.to_i
来源：http://uwm.yongpay.top

C#:   (int)resp.StatusCode
来源：http://hrj.yfazqb.com

[L08] 并发请求多个地址
来源：http://tpt.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lzc.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://ppz.redwolf501.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zla.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hmd.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xtj.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://knf.quarkkingdee.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vcu.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yqx.yanxiufei.cn

================================================================================
来源：http://ter.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://ewn.birdmap.top

================================================================================
来源：http://uxh.yongpay.top

[M01] 读取命令行参数
来源：http://btx.yueranfly.top

Py:   sys.argv[1:]
来源：http://rwl.haohaochexian.top

PHP:  $argv;  $argc;
来源：http://mng.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://uco.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://vqr.yj20258.top

Java: args 数组（main 方法参数）
来源：http://pgh.zhoulong.xyz

Go:   os.Args[1:]
来源：http://gig.sufxvd.cn

Ruby: ARGV
来源：http://evn.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://hlv.zhixingplan.top

[M02] 读取环境变量
来源：http://scs.cashguo.top

Py:   os.environ.get("HOME")
来源：http://gox.fengsongda.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ujt.9152youxi.cn

JS:   process.env.HOME
来源：http://fxy.ivvv.top

TS:   process.env.HOME
来源：http://rhi.shanyushiyangtech.top

Java: System.getenv("HOME")
来源：http://kfn.xziqi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aaj.hesvh.cn

Ruby: ENV["HOME"]
来源：http://rio.zhiwuduotai.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qxi.yongpay.top

[M03] 执行外部命令
来源：http://csf.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ykj.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xyq.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://eux.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cpj.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sxp.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://baa.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ufi.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://uxv.aibaodan.cn

[M04] 获取当前工作目录
来源：http://gjb.sweek.top

Py:   os.getcwd()
来源：http://tzf.vqdsnc.cn

PHP:  getcwd();
来源：http://zft.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://ojv.jinqigufen.top

TS:   process.cwd()
来源：http://yil.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://hmp.cucudq.cn

Go:   os.Getwd()
来源：http://qfh.zdbjq.cn

Ruby: Dir.pwd
来源：http://sxf.hywenlv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tvb.ybcxt.top

[M05] 设置退出码
来源：http://dfk.gzhubu.top

Py:   sys.exit(1)
来源：http://jgs.meibo888.top

PHP:  exit(1);
来源：http://wra.hongshengwenyu.top

JS:   process.exit(1)
来源：http://fnd.meibo888.top

TS:   process.exit(1)
来源：http://isz.bjfxy.top

Java: System.exit(1)
来源：http://hdf.bjfxy.top

Go:   os.Exit(1)
来源：http://tec.hammf.cn

Ruby: exit 1
来源：http://bpp.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iwr.jinqigufen.top

[M06] 向标准错误输出
来源：http://nsz.xziqi.cn

Py:   print("err", file=sys.stderr)
来源：http://hqn.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://ycz.sysykeji.top

JS:   console.error("err")
来源：http://uvz.ydzc1.top

TS:   console.error("err")
来源：http://hxt.yvedp.cn

Java: System.err.println("err")
来源：http://osd.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cub.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://tor.zhengqikj.top

C#:   Console.Error.WriteLine("err")
来源：http://scr.c1oappe.top

[M07] 判断是否为主入口
来源：http://irg.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://kan.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rro.ctjpmb.com

JS:   require.main === module
来源：http://ipw.0kj1m.cn

TS:   require.main === module
来源：http://rcm.sufxvd.cn

Java: public static void main(String[] args)
来源：http://tgr.uphjek.com

Go:   func main()
来源：http://llz.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zbu.bbcook.cn

C#:   static void Main(string[] args)
来源：http://vaz.zhaomingkeji.xyz

[M08] 获取系统与运行时信息
来源：http://kjq.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://wva.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://zqe.smart0.xyz

JS:   process.platform;  process.version
来源：http://aaq.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://ojd.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://azr.xuetiantiany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://toa.nanxinkj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tkj.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://yzw.fanxiaobao.xyz

================================================================================
来源：http://tzm.zhixingplan.top

N. 数据结构与算法
来源：http://cac.sweek.top

================================================================================
来源：http://gel.sxryk.cn

[N01] 二分查找（有序数组）
来源：http://fwb.wangdashe.top

Py:   bisect.bisect_left(arr, x)
来源：http://imi.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nci.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://agd.ivvv.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ynx.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qwy.jinghuilouyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://jtg.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dhh.hesvh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wng.yj20258888.top

[N02] 排序（工程实践用内置实现）
来源：http://muu.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://zkr.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yuq.ivvv.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fka.andypj.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://qxz.epnwcf.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cgg.yanxiufei.cn

Go:   slices.Sort(arr)
来源：http://dxm.vehdjk.com

Ruby: arr.sort
来源：http://kod.c1oappe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://buf.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://smq.yvedp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xzl.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://ash.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sdo.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mvd.haohaochexian.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qik.redwolf501.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mao.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yop.zhoulong.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://zxp.gaohongyu789.top

[N04] 斐波那契数列
来源：http://sdh.hfpthk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://neo.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://liu.nanxuanxn.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ylw.zhongyouzk.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cvt.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://psn.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://esq.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nys.yj20258.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ukr.gaohongyu789.top

[N05] 最大公约数
来源：http://zvv.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://zeq.jianghu66.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hkn.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://szo.yongpay.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sbs.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ovy.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yoo.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://xaf.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kdz.vehdjk.com

[N06] 判断回文字符串
来源：http://gio.jlsjyb.cn

Py:   s == s[::-1]
来源：http://zyj.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://ems.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://aki.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://uss.vehdjk.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cuo.chenlongwang.top

Go:   // 双指针从两端比较
来源：http://rip.gotoacloud.top

Ruby: s == s.reverse
来源：http://zbb.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ppu.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://rjx.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://psk.0kj1m.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ykd.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lzb.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://qag.sufxvd.cn

Java: // 手写 HashMap
来源：http://ijh.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://mgm.jyoumei.cn

Ruby: // 手写 Hash
来源：http://otb.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://sqr.yvedp.cn

[N08] 生成全排列
来源：http://seu.tarul.cn

Py:   itertools.permutations(arr)
来源：http://nlu.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://pgs.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://dfb.yuxming.cn

TS:   // 手写回溯递归
来源：http://tiw.aizwys.cn

Java: // 手写回溯递归
来源：http://slz.jyoumei.cn

Go:   // 手写回溯递归
来源：http://iir.xinyue.icu

Ruby: arr.permutation.to_a
来源：http://otz.xziqi.cn

C#:   // 手写回溯递归
来源：http://qkr.xinyue.icu

[N09] 栈与队列
来源：http://yau.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zga.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://izk.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kxc.c1oappe.top


<!-- 参考信息 -->