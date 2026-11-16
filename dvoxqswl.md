代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bso.ctjpmb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tdz.uphjek.com

JS:   JSON.stringify(obj)
来源：http://eud.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://xkn.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tqj.vehdjk.com

Go:   json.Marshal(obj)
来源：http://ort.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://ags.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://jnh.yuanzhike.top

[K02] JSON 字符串转对象
来源：http://vey.jianghu66.top

Py:   json.loads(s)
来源：http://sgz.xuanzx.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ppw.epnwcf.com

JS:   JSON.parse(s)
来源：http://tai.sjlbkw.cn

TS:   JSON.parse(s)
来源：http://gtq.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nwz.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://wcd.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://ocb.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wnm.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://uxj.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mil.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kgw.chenjidiqi.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://iwf.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vjn.xuetiantiany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://syf.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jld.jqgufenzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://ynl.9152youxi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hwz.xuanzx.com

[K04] 读取 JSON 文件
来源：http://wgy.cucudq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fpc.snrcjt.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hle.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fos.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oro.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eof.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yrn.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eqk.uphjek.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sop.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://juj.zdqjudy.top

Py:   copy.deepcopy(obj)
来源：http://thb.gogol.net.cn

PHP:  unserialize(serialize($obj));
来源：http://qka.yueranfly.top

JS:   structuredClone(obj)
来源：http://kih.zhoulong.xyz

TS:   structuredClone(obj)
来源：http://jtv.jinqigufen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tck.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hqx.shanyushiyangtech.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xms.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nos.fehbvm.com

[K06] 解析 URL 查询串
来源：http://osi.fzhhl.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ajz.ppjwa.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fwp.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://djn.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ddr.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jxg.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://smz.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nkm.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mbr.shzxlz.cn

[K07] 进制转换
来源：http://fht.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lvs.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://edt.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fql.sufxvd.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cqj.gzhubu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pow.andypj.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yfe.jinqigfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wkh.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rrv.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://ezk.hammf.cn

Py:   pickle.dumps(obj)
来源：http://rdn.hammf.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mln.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://zmy.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://ylj.yonumen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bgb.chenzaomai.com

Go:   encoding/gob
来源：http://vnr.birdmap.top

Ruby: Marshal.dump(obj)
来源：http://tai.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gpn.fanxiaobao.xyz

================================================================================
来源：http://buq.fanxiaobao.xyz

L. 网络请求
来源：http://zyj.yvedp.cn

================================================================================
来源：http://hxn.jqgufenzy.top

[L01] 发送 GET 请求
来源：http://qji.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wob.xuanzx.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hqh.shangyingyoupin.top

JS:   await fetch(url)
来源：http://grw.aizwys.cn

TS:   await fetch(url)
来源：http://obu.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nae.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://skc.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://umc.yonumen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://onz.fanxiaobao.xyz

[L02] 发送 POST JSON
来源：http://eyb.hesvh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pbe.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hio.gogol.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ulo.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nhq.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://til.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ckc.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://szr.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jqi.chenlongwang.top

[L03] 设置自定义请求头
来源：http://tyu.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kml.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qmg.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://utk.yvedp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bms.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kpx.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qal.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cph.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://anr.quarkkingdee.top

[L04] 设置超时
来源：http://szc.c1oappe.top

Py:   requests.get(url, timeout=5)
来源：http://ohs.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nsn.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cyo.xuanzx.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yis.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ufm.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jhm.wangshuangyany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eyk.yuxming.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dia.vehdjk.com

[L05] 上传文件（multipart）
来源：http://jcu.jianghu66.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kdr.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ztf.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ecw.meibo888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tyl.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uzb.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rxs.zdbjq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jqu.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jsk.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://own.jiagoushi.top

Py:   resp.json()
来源：http://sdg.jqgfzy.top

PHP:  json_decode($body, true);
来源：http://vat.guowangkeji.top

JS:   await resp.json()
来源：http://qtj.uphjek.com

TS:   await resp.json()
来源：http://zln.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lho.xingfuxueyuan.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nev.vehdjk.com

Ruby: JSON.parse(resp.body)
来源：http://mkm.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nog.xziqi.cn

[L07] 处理 HTTP 状态码
来源：http://gjd.fehbvm.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://huy.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ana.yanxiufei.cn

JS:   resp.ok;  resp.status
来源：http://fxo.aizwys.cn

TS:   resp.ok;  resp.status
来源：http://qhh.jqgufenzy.top

Java: resp.statusCode()
来源：http://feb.xylfe.cn

Go:   resp.StatusCode
来源：http://fmp.52xcode.cn

Ruby: resp.code.to_i
来源：http://wyo.zdqjudy.top

C#:   (int)resp.StatusCode
来源：http://jos.fehbvm.com

[L08] 并发请求多个地址
来源：http://ons.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hrg.ywan-chungtsiang.top

PHP:  curl_multi_init() 系列
来源：http://vef.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://phb.epnwcf.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ayx.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ioj.hesvh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://stz.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fpb.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ayg.mhx1999.top

================================================================================
来源：http://vrh.nanxinkj.top

M. 命令行 / 进程 / 环境
来源：http://yjh.kuanghao11.cn

================================================================================
来源：http://xif.cheryme.top

[M01] 读取命令行参数
来源：http://ihi.jyoumei.cn

Py:   sys.argv[1:]
来源：http://qoj.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://hrs.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://olx.hammf.cn

TS:   process.argv.slice(2)
来源：http://lil.tarul.cn

Java: args 数组（main 方法参数）
来源：http://kfp.epnwcf.com

Go:   os.Args[1:]
来源：http://whm.kuanghao11.cn

Ruby: ARGV
来源：http://teg.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://rly.gzhubu.top

[M02] 读取环境变量
来源：http://axd.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://xfl.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rmp.shuidangran.top

JS:   process.env.HOME
来源：http://luj.wangdashe.top

TS:   process.env.HOME
来源：http://ppu.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://gfm.tianlin.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gri.zdqjudy.top

Ruby: ENV["HOME"]
来源：http://dbd.zhoulong.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aau.cheryme.top

[M03] 执行外部命令
来源：http://bgt.hammf.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hoi.52xcode.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jhy.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://emq.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bhc.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ocd.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hlu.chenlongwang.top

Ruby: system("ls -l");  `ls -l`
来源：http://soj.shanyushiyangtech.top

C#:   Process.Start("ls", "-l");
来源：http://sqs.quarkkingdee.top

[M04] 获取当前工作目录
来源：http://xia.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://vvm.iojbl.cn

PHP:  getcwd();
来源：http://luy.pengpengdd.cyou

JS:   process.cwd()
来源：http://qfq.xinyue.icu

TS:   process.cwd()
来源：http://djy.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://ybw.nwbrower.top

Go:   os.Getwd()
来源：http://mfa.quarkkingdee.top

Ruby: Dir.pwd
来源：http://pvm.hesvh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gqg.shuidangran.top

[M05] 设置退出码
来源：http://teg.nanxinkj.top

Py:   sys.exit(1)
来源：http://tqp.hesvh.cn

PHP:  exit(1);
来源：http://uvp.pycfn.com

JS:   process.exit(1)
来源：http://mpn.quarkkingdee.top

TS:   process.exit(1)
来源：http://znk.9152youxi.cn

Java: System.exit(1)
来源：http://ulp.0kj1m.cn

Go:   os.Exit(1)
来源：http://kxy.zdbjq.cn

Ruby: exit 1
来源：http://zhx.cucudq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qoh.vqdsnc.cn

[M06] 向标准错误输出
来源：http://zbc.redwolf501.top

Py:   print("err", file=sys.stderr)
来源：http://hci.yj20258.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ztl.snrcjt.cn

JS:   console.error("err")
来源：http://wof.snrcjt.cn

TS:   console.error("err")
来源：http://ruy.zhoulong.xyz

Java: System.err.println("err")
来源：http://lxx.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pvi.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://mxx.ehwqpu.com

C#:   Console.Error.WriteLine("err")
来源：http://gkr.jqgufenzy.top

[M07] 判断是否为主入口
来源：http://bit.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://pgt.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dnj.yj202588.top

JS:   require.main === module
来源：http://git.yueranfly.top

TS:   require.main === module
来源：http://fld.hcnkem.com

Java: public static void main(String[] args)
来源：http://pxe.cdnleiting.top

Go:   func main()
来源：http://mro.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fgb.fengsongda.top

C#:   static void Main(string[] args)
来源：http://pwn.yj20258.top

[M08] 获取系统与运行时信息
来源：http://fwn.xziqi.cn

Py:   platform.system();  platform.python_version()
来源：http://qme.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://uxk.jianghu66.top

JS:   process.platform;  process.version
来源：http://zvn.daxiang520.top

TS:   process.platform;  process.version
来源：http://nhm.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hna.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://uuq.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://inu.chenzaomai.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ksy.sysykeji.top

================================================================================
来源：http://rfx.cdnleiting.top

N. 数据结构与算法
来源：http://gfj.quarkkingdee.top

================================================================================
来源：http://euc.tanke756.top

[N01] 二分查找（有序数组）
来源：http://inn.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://fyh.zhengqikj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://udm.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wck.hcnkem.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bzh.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://mvq.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://qfw.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ibr.vehdjk.com

C#:   Array.BinarySearch(arr, x)
来源：http://opx.fktsv.cn

[N02] 排序（工程实践用内置实现）
来源：http://dzy.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://vat.cheryme.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mly.zhengqikj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zcy.hongshengwenyu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ihb.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cbb.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://cgq.hywenlv.cn

Ruby: arr.sort
来源：http://mrk.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dty.zhijiandao.cn

[N03] 快速排序（分治示例）
来源：http://kke.uphjek.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tly.xuanzx.com

PHP:  // 递归实现，或用 usort
来源：http://yqz.pengpengdd.cyou

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ofc.shuidangran.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qxj.sxryk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mge.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ntq.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://olu.svipenyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tor.shangyingyoupin.top

[N04] 斐波那契数列
来源：http://jzg.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fon.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://juf.zycfv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wms.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fni.jinghuilouyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ggz.ybcxt.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cvf.gzhubu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xhq.sufxvd.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zsn.chenlongwang.top

[N05] 最大公约数
来源：http://yoz.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://btn.feifeiyinyue.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mtn.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pxl.pengpengdd.cyou

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bod.jyoumei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dnm.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cvi.yuxming.cn

Ruby: a.gcd(b)
来源：http://qfn.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://itu.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://ajz.wangshuangyany.cn

Py:   s == s[::-1]
来源：http://qak.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://uoe.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://xeg.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://hmt.jinqigufen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gjq.fktsv.cn

Go:   // 双指针从两端比较
来源：http://vbe.tian-w.cn

Ruby: s == s.reverse
来源：http://zte.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kgs.zdbjq.cn

[N07] 两数之和（返回下标）
来源：http://itn.hywenlv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ovd.zhengqikj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zbo.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://yqk.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://ifr.cucudq.cn

Java: // 手写 HashMap
来源：http://eef.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://prb.jinqigfzy.top

Ruby: // 手写 Hash
来源：http://eno.hammf.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hja.birdmap.top

[N08] 生成全排列
来源：http://nvt.ivvv.top

Py:   itertools.permutations(arr)
来源：http://ivi.smart0.xyz

PHP:  // 手写递归交换
来源：http://bob.tian-w.cn

JS:   // 手写回溯递归
来源：http://wkd.ivvv.top

TS:   // 手写回溯递归
来源：http://oya.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://uhp.hesvh.cn

Go:   // 手写回溯递归
来源：http://zjz.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://hnp.shanyushiyangkeji.top

C#:   // 手写回溯递归
来源：http://cjs.ehwqpu.com

[N09] 栈与队列
来源：http://jsy.yj202588.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hlk.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sxr.ctjpmb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://udz.zhixingplan.top


<!-- 参考信息 -->