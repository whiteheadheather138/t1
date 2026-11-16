代发 wailian999

Ruby: attr_accessor :name
来源：http://bac.hywenlv.cn

C#:   public string Name { get; set; }
来源：http://yji.zhiwuduotai.top

[G12] 对象转字符串
来源：http://xbu.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://yxv.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nrm.xuetiantiany.cn

JS:   toString() { return this.name; }
来源：http://zcq.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://hdr.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://lvb.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://qii.svipenyu.cn

Ruby: def to_s; @name; end
来源：http://lse.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://xcv.jinqigfzy.top

[G13] 判断对象类型
来源：http://jef.yuanzhike.top

Py:   isinstance(u, User)
来源：http://kut.yangfankeji.com

PHP:  $u instanceof User
来源：http://vrc.jyoumei.cn

JS:   u instanceof User
来源：http://eag.shzxlz.cn

TS:   u instanceof User
来源：http://aod.yueranfly.top

Java: u instanceof User
来源：http://lec.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://cdg.ydjk.org.cn

Ruby: u.is_a?(User)
来源：http://eox.bbcook.cn

C#:   u is User
来源：http://qur.yueranfly.top

[G14] 数据类 / record
来源：http://qjc.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dcp.daxiang520.top

PHP:  // 用 readonly 属性模拟
来源：http://mvm.havefunace.top

JS:   // 无内置：普通类或对象字面量
来源：http://vcx.kuanghao11.cn

TS:   type User = { name: string; age: number };
来源：http://qas.svipenyu.cn

Java: record User(String name, int age) {}
来源：http://wvz.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://kjx.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ygr.snrcjt.cn

C#:   record User(string Name, int Age);
来源：http://idr.yfazqb.com

[G15] 枚举
来源：http://ikx.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yzg.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://skg.shuidangran.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vqb.fzhhl.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://utx.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://yoa.yfazqb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://biv.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://uic.jqgufenzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cbq.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://fba.yj20258.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lgu.xziqi.cn

PHP:  get_object_vars($obj);
来源：http://evx.havefunace.top

JS:   Object.entries(obj)
来源：http://zcl.nanxinkj.top

TS:   Object.entries(obj)
来源：http://tfr.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dpv.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zgl.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://rpp.yj202588.top

C#:   // 用反射或 System.Text.Json
来源：http://lyw.wangdashe.top

================================================================================
来源：http://khn.zhengqikj.top

H. 异常与错误处理
来源：http://vsv.andypj.xyz

================================================================================
来源：http://bdf.cdnleiting.top

[H01] try / catch 基础
来源：http://wif.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hyb.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iir.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ppi.pengpengdd.cyou

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wch.iojbl.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ptt.meibo888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gfq.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oil.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ngn.yuxming.cn

[H02] finally / ensure 收尾
来源：http://ohw.dashuyun.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pzx.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cit.uphjek.com

JS:   try { f(); } finally { cleanup(); }
来源：http://sdo.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bpv.feifeiyinyue.top

Java: try { f(); } finally { cleanup(); }
来源：http://vlj.pengpengdd.cyou

Go:   defer cleanup()             // 函数返回时执行
来源：http://aiz.cqqwz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cit.9152youxi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jrs.hongshengwenyu.top

[H03] 主动抛出异常
来源：http://csm.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://ypl.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://htv.jqgfzy.top

JS:   throw new Error("错误信息");
来源：http://vzs.havefunace.top

TS:   throw new Error("错误信息");
来源：http://iyp.gogol.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jnc.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gwx.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oul.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://edg.zhaomingkeji.xyz

[H04] 自定义异常类型
来源：http://psn.zhoulong.xyz

Py:   class MyError(Exception): pass
来源：http://kmj.yuxming.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nkz.fktsv.cn

JS:   class MyError extends Error {}
来源：http://rei.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://qko.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://yqf.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jnz.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://bww.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://eqq.dianchejie.cn

[H05] 捕获特定类型
来源：http://shm.sxryk.cn

Py:   except ValueError as e:
来源：http://ekv.zdqjudy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ujk.fzhhl.top

JS:   if (e instanceof TypeError) {}
来源：http://oem.hysaishi.cn

TS:   if (e instanceof TypeError) {}
来源：http://hmd.gogol.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://vvv.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gsv.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://djh.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yrm.feifeiyinyue.top

[H06] 可选值 / 空值安全访问
来源：http://ncn.sweek.top

Py:   value = d.get("k") or default
来源：http://cpy.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://eow.smart0.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://urz.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://gon.andypj.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qii.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tsp.wangshuangyany.cn

Ruby: d&.dig(:a, :b)
来源：http://dzn.smart0.xyz

C#:   obj?.A?.B ?? default
来源：http://mvg.zdqjudy.top

[H07] 断言
来源：http://xcc.sweek.top

Py:   assert x > 0, "必须为正"
来源：http://blg.dianchejie.cn

PHP:  assert($x > 0);
来源：http://svd.guowangkeji.top

JS:   console.assert(x > 0);
来源：http://lfq.feifeiyinyue.top

TS:   console.assert(x > 0);
来源：http://tfa.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://bpd.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ssj.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sur.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://agw.0kj1m.cn

[H08] 获取错误信息与堆栈
来源：http://cbz.xziqi.cn

Py:   str(e);  traceback.format_exc()
来源：http://mdw.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qrc.daxiang520.top

JS:   e.message;  e.stack
来源：http://you.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kdh.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tmv.jqgfzy.top

Go:   err.Error()
来源：http://kln.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://vjx.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://whl.daria6918.cn

[H09] 带错误码的异常
来源：http://ofh.hammf.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://axo.52xcode.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gth.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xjv.smart0.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hfp.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bmp.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ngn.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ahy.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lmx.zhoulong.xyz

[H10] 资源自动释放
来源：http://xlf.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qje.vqdsnc.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fys.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bev.zhoulong.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qqk.jinqigfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wsy.daria6918.cn

Go:   defer f.Close()
来源：http://osv.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ygv.hywenlv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iyc.gzhubu.top

================================================================================
来源：http://mym.xziqi.cn

I. 正则表达式
来源：http://qhw.wangdashe.top

================================================================================
来源：http://vnf.sufxvd.cn

[I01] 判断是否匹配
来源：http://koj.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://phg.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://mgk.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://qrd.nanxuanxn.top

TS:   /\d+/.test(s)
来源：http://vao.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xkr.daria6918.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jdv.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://njz.9152youxi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gjp.gotoacloud.top

[I02] 提取所有匹配
来源：http://pgs.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://nbv.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cmj.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uay.jianghu66.top

TS:   s.match(/\d+/g)
来源：http://kxr.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rfa.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aah.gotoacloud.top

Ruby: s.scan(/\d+/)
来源：http://jqf.jlsjyb.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cxu.cdnleiting.top

[I03] 提取捕获分组
来源：http://gds.hywenlv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uqa.yj202588.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://csp.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wcv.fanxiaobao.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dfo.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dod.cheryme.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oem.zhengqikj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://biv.yfazqb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sxq.9152youxi.cn

[I04] 正则替换
来源：http://jfn.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dat.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cyj.zhaomingkeji.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://nls.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://qlu.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kom.yj20258.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cdx.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://fvn.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uvl.jinqigufen.top

[I05] 按正则拆分
来源：http://ovj.shanyushiyangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pdy.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ncl.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://yde.zhengqikj.top

TS:   s.split(/\s*,\s*/)
来源：http://oym.hcnkem.com

Java: s.split("\\s*,\\s*")
来源：http://qii.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wit.zhijiandao.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mrd.vehdjk.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lsc.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sdk.jinyuanbaomall.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bis.yuanzhike.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://shn.jqgfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ahz.sjlbkw.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mqq.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xoo.tarul.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yma.cucudq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wfu.ppjwa.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qrl.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://fza.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cfs.pengpengdd.cyou

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ohv.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kzr.jinghuilouyu.cn

TS:   /error/gim
来源：http://iza.9152youxi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://asx.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yms.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://iiq.svipenyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://neu.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://ary.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xfr.jiagoushi.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zwi.dianchejie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jgx.chenjidiqi.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eha.zdqjudy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xau.hnxiangtu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zxl.fanxiaobao.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kxb.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gnb.jqgufenzy.top

================================================================================
来源：http://zdx.xingfuxueyuan.xyz

J. 日期与时间
来源：http://ich.dianchejie.cn

================================================================================
来源：http://lhy.sjlbkw.cn

[J01] 获取当前时间
来源：http://dvw.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://npr.guannengcc.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dws.cqqwz.cn

JS:   new Date();  Date.now()
来源：http://dlv.hywenlv.cn

TS:   new Date();  Date.now()
来源：http://xov.cucudq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xpq.guowangkeji.top

Go:   time.Now()
来源：http://ahn.pengpengdd.cyou

Ruby: Time.now
来源：http://zic.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iuy.chenlongwang.top

[J02] 格式化输出
来源：http://cpq.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pqn.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://upl.vqdsnc.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ltc.jiagoushi.top

TS:   d.toISOString()
来源：http://svr.gzhubu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bjk.zhengqikj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iux.yj20258.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cpg.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://krc.ydjk.org.cn

[J03] 字符串解析为日期
来源：http://sjr.dashuyun.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nch.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://glw.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://rmv.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://wmj.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://olz.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zbn.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://txl.wangdashe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wie.yj202588.top

[J04] 时间戳与日期互转
来源：http://iyl.ivvv.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bej.snrcjt.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qwb.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ygw.sweek.top

TS:   Math.floor(Date.now() / 1000)
来源：http://slc.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bcm.jyoumei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vyu.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ddo.xziqi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jtl.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://bfr.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://gzi.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vpp.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://inh.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wft.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://cyz.tarul.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ppf.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://ynj.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://isx.cdnleiting.top

[J06] 计算两时间之差
来源：http://jcw.aibaodan.cn

Py:   (end - start).total_seconds()
来源：http://yxh.yuxming.cn

PHP:  $end->diff($start)->days;
来源：http://jxo.tanke756.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vyd.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://knb.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fcp.andypj.xyz

Go:   end.Sub(start).Hours()
来源：http://sov.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://hlv.0kj1m.cn

C#:   (end - start).TotalSeconds
来源：http://omt.shanyushiyangtech.top

[J07] 比较两个日期
来源：http://vmt.zhoulong.xyz

Py:   d1 < d2;  d1 == d2
来源：http://jfu.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kvl.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://rzb.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zzv.9152youxi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://exi.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wyl.ehwqpu.com

Ruby: d1 < d2;  d1 == d2
来源：http://lsv.snrcjt.cn

C#:   d1 < d2;  d1 == d2
来源：http://msx.fzhhl.top

[J08] 提取年月日与星期
来源：http://urf.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nlu.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jaw.yj20258.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ndg.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cld.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sxv.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lob.nanxuanxn.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ubp.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lat.hammf.cn

[J09] 时区处理
来源：http://csw.zhoulong.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qpn.cqqwz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mws.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ism.havefunace.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wwx.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lsk.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gxx.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ysg.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aoh.shangyingyoupin.top

[J10] 取今天 / 本月第一天
来源：http://oqq.vehdjk.com


<!-- 参考信息 -->