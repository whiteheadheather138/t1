代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://zdj.tanke756.top

JS:   toString() { return this.name; }
来源：http://cuc.jinghuilouyu.cn

TS:   toString(): string { return this.name; }
来源：http://vzb.bjfxy.top

Java: @Override public String toString() { return name; }
来源：http://gat.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lpz.hammf.cn

Ruby: def to_s; @name; end
来源：http://vjq.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://pem.guowangkeji.top

[G13] 判断对象类型
来源：http://mxz.xinyue.icu

Py:   isinstance(u, User)
来源：http://ruo.wangdashe.top

PHP:  $u instanceof User
来源：http://kea.bjfxy.top

JS:   u instanceof User
来源：http://lld.fanxiaobao.xyz

TS:   u instanceof User
来源：http://ddr.guannengcc.top

Java: u instanceof User
来源：http://lbq.haohaochexian.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://aav.fengsongda.top

Ruby: u.is_a?(User)
来源：http://ltu.aibaodan.cn

C#:   u is User
来源：http://qhq.redwolf501.top

[G14] 数据类 / record
来源：http://oob.sufxvd.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ivg.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://xxk.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://jjd.kuanghao11.cn

TS:   type User = { name: string; age: number };
来源：http://jqi.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://epm.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://gtx.cdnleiting.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ull.zhiwuduotai.top

C#:   record User(string Name, int Age);
来源：http://cnl.pengpengdd.cyou

[G15] 枚举
来源：http://ftd.c1oappe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jqo.andypj.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://cur.feifeiyinyue.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hep.hfpthk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hkl.daxiang520.top

Java: enum Color { RED, GREEN }
来源：http://usf.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qtq.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://vuc.fzhhl.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yco.gogol.net.cn

[G16] 对象转数组 / 字典
来源：http://vwg.yj20258888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qrr.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://vpa.fengsongda.top

JS:   Object.entries(obj)
来源：http://nxi.yj20258.top

TS:   Object.entries(obj)
来源：http://mnw.zhiwuduotai.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qxk.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yaa.ydjk.org.cn

Ruby: obj.instance_variables
来源：http://ncd.tanke756.top

C#:   // 用反射或 System.Text.Json
来源：http://xbj.zhengqikj.top

================================================================================
来源：http://erv.jyoumei.cn

H. 异常与错误处理
来源：http://cou.nwbrower.top

================================================================================
来源：http://byl.gzhubu.top

[H01] try / catch 基础
来源：http://ilb.chenzaomai.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://twb.yfazqb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rxc.chenzaomai.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vqx.xuetiantiany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zkz.jyoumei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nvz.ydjk.org.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://seu.aizwys.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cts.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ybf.yangfankeji.com

[H02] finally / ensure 收尾
来源：http://new.cucudq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jzz.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zfj.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://fjt.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mke.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://gqr.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://zlf.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yxs.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qiu.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://zxj.yj20258888.top

Py:   raise ValueError("错误信息")
来源：http://nff.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ujm.yongpay.top

JS:   throw new Error("错误信息");
来源：http://yec.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://fzt.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ngy.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cwr.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wep.svipenyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hlz.xuanzx.com

[H04] 自定义异常类型
来源：http://bcf.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://ayj.snrcjt.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ljc.yj20258888.top

JS:   class MyError extends Error {}
来源：http://vjd.52xcode.cn

TS:   class MyError extends Error {}
来源：http://err.tianlin.xyz

Java: class MyException extends RuntimeException {}
来源：http://ncs.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gcm.cheryme.top

Ruby: class MyError < StandardError; end
来源：http://bor.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://bkq.zhijiandao.cn

[H05] 捕获特定类型
来源：http://hno.hammf.cn

Py:   except ValueError as e:
来源：http://sdd.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cbm.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://kfk.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://tqi.tanke756.top

Java: catch (IOException | SQLException e) {}
来源：http://sgb.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xlx.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://jky.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://btf.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://ecy.havefunace.top

Py:   value = d.get("k") or default
来源：http://xbz.zhongyouzk.top

PHP:  $v = $d["k"] ?? null;
来源：http://qbx.gzhubu.top

JS:   obj?.a?.b;  d ?? default
来源：http://gbh.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://xvu.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://apv.vehdjk.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ope.yfazqb.com

Ruby: d&.dig(:a, :b)
来源：http://jtj.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://zlp.guowangkeji.top

[H07] 断言
来源：http://mbn.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://oux.yfazqb.com

PHP:  assert($x > 0);
来源：http://uii.yonumen.top

JS:   console.assert(x > 0);
来源：http://ovb.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://jrs.jyoumei.cn

Java: assert x > 0 : "必须为正";
来源：http://ljl.shanyushiyangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tfi.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://lut.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://erw.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://kqy.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://xax.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fil.zdqjudy.top

JS:   e.message;  e.stack
来源：http://ukc.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ugr.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://peg.ybcxt.top

Go:   err.Error()
来源：http://fhv.jinqigufen.top

Ruby: e.message;  e.backtrace
来源：http://qok.jqgfzy.top

C#:   e.Message;  e.StackTrace
来源：http://bcn.shzxlz.cn

[H09] 带错误码的异常
来源：http://ybi.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nuu.zhoulong.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://rdh.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ayg.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://son.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uom.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bis.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zrv.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ucp.shangyingyoupin.top

[H10] 资源自动释放
来源：http://cbv.zhixingplan.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dzc.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lml.hnqzz.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yst.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tbd.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kwh.birdmap.top

Go:   defer f.Close()
来源：http://jgd.bjfxy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://avq.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://beb.shanyushiyangtech.top

================================================================================
来源：http://fvk.gzhubu.top

I. 正则表达式
来源：http://mrm.jlsjyb.cn

================================================================================
来源：http://zkj.hysaishi.cn

[I01] 判断是否匹配
来源：http://ouu.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qgg.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://inc.ybcxt.top

JS:   /\d+/.test(s)
来源：http://njj.yonumen.top

TS:   /\d+/.test(s)
来源：http://yoe.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://epu.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pos.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://bzz.svipenyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jvn.hywenlv.cn

[I02] 提取所有匹配
来源：http://ffp.cdnleiting.top

Py:   re.findall(r"\d+", s)
来源：http://omf.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hvg.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mog.hnxiangtu.top

TS:   s.match(/\d+/g)
来源：http://shy.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ujf.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bsp.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://xhu.xuetiantiany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nni.zhoulong.xyz

[I03] 提取捕获分组
来源：http://jzn.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://omp.dashuyun.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ajy.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gpy.fanxiaobao.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bvw.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fly.daxiang520.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bey.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://utm.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://coz.ybcxt.top

[I04] 正则替换
来源：http://asz.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xaz.zdbjq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rew.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://rgg.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://nmj.fktsv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ypp.jinqigufen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ugi.jianghu66.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zwx.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oip.shangyingyoupin.top

[I05] 按正则拆分
来源：http://hcw.zdqjudy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wxa.yj20258.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wil.gotoacloud.top

JS:   s.split(/\s*,\s*/)
来源：http://jxb.vqdsnc.cn

TS:   s.split(/\s*,\s*/)
来源：http://fzv.yongpay.top

Java: s.split("\\s*,\\s*")
来源：http://gce.guannengcc.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pyg.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://vvr.zycfv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://znz.zhiwuduotai.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://krz.birdmap.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fuv.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ouo.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yja.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sfi.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sge.sysykeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tkj.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pfe.gogol.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://srd.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://daw.pengpengdd.cyou

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ory.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ack.ehwqpu.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yao.hnxiangtu.top

TS:   /error/gim
来源：http://mun.ctjpmb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ely.tianlin.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pvo.hammf.cn

Ruby: s.scan(/error/i)
来源：http://vki.chenzaomai.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://esm.meibo888.top

[I08] 贪婪与非贪婪匹配
来源：http://hxj.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cpt.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hew.gotoacloud.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wpk.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jsu.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://zwb.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kbl.tanke756.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iph.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sbb.aibaodan.cn

================================================================================
来源：http://nlr.xuanzx.com

J. 日期与时间
来源：http://plx.cqqwz.cn

================================================================================
来源：http://hdp.kuanghao11.cn

[J01] 获取当前时间
来源：http://jsy.jiagoushi.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://afw.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dha.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://lle.jlsjyb.cn

TS:   new Date();  Date.now()
来源：http://btp.yvedp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pzo.zhixingplan.top

Go:   time.Now()
来源：http://tgp.zhoulong.xyz

Ruby: Time.now
来源：http://tdt.nwbrower.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fqg.tanke756.top

[J02] 格式化输出
来源：http://oqk.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cid.yfazqb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ufw.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lbo.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://cnn.zhiwuduotai.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zdj.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nmh.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wpf.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ifr.ehwqpu.com

[J03] 字符串解析为日期
来源：http://zhl.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nkj.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hek.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://ouz.gogol.net.cn

TS:   new Date("2024-01-02")
来源：http://sza.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://rmf.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mdx.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://bmb.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kra.hfpthk.cn

[J04] 时间戳与日期互转
来源：http://nrb.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sfx.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jvn.birdmap.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oho.chenzaomai.com

TS:   Math.floor(Date.now() / 1000)
来源：http://iwv.ppjwa.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://unb.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tvf.sysykeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://air.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pym.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://bbk.fzhhl.top

Py:   now + timedelta(days=7)
来源：http://yuz.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://naj.xylfe.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nyl.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zun.jqgfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://hbv.gzhubu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pkb.nwbrower.top

Ruby: Time.now + 7 * 86400
来源：http://kia.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://meo.snrcjt.cn

[J06] 计算两时间之差
来源：http://mcd.zdbjq.cn

Py:   (end - start).total_seconds()
来源：http://iom.9152youxi.cn

PHP:  $end->diff($start)->days;
来源：http://hrs.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://olr.fzhhl.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kac.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lju.jqgfzy.top

Go:   end.Sub(start).Hours()
来源：http://jgl.fengsongda.top

Ruby: end - start                 # 返回秒数
来源：http://zet.jinghuilouyu.cn

C#:   (end - start).TotalSeconds
来源：http://dko.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://wwn.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://kxf.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kzo.vehdjk.com

JS:   d1.getTime() < d2.getTime()
来源：http://qud.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://apn.yongpay.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kft.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kcj.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://wso.ybcxt.top

C#:   d1 < d2;  d1 == d2
来源：http://ndr.sweek.top

[J08] 提取年月日与星期
来源：http://xuv.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xcy.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kek.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lkz.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nrn.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fxb.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aqv.zhaomingkeji.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jiw.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mod.nanxuanxn.top

[J09] 时区处理
来源：http://typ.birdmap.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lbt.hnxiangtu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://isr.kuanghao11.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sai.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eue.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rmq.shangyingyoupin.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://orb.epnwcf.com

Ruby: Time.now.getlocal("+08:00")
来源：http://wxx.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cnr.bjfxy.top

[J10] 取今天 / 本月第一天
来源：http://lan.mhx1999.top

Py:   date.today();  date.today().replace(day=1)
来源：http://oll.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mox.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hst.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://amq.hongshengwenyu.top


<!-- 参考信息 -->