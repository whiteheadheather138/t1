代发 wailian999

SHOW INDEX FROM users;
来源：http://yow.yfazqb.com

[Q73] 查看表状态
来源：http://liv.xinyue.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://lco.jiagoushi.top

[Q74] 强制使用索引
来源：http://ela.mhx1999.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aej.vqdsnc.cn

[Q75] 日期格式化
来源：http://iib.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://udj.ywan-chungtsiang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vdr.cucudq.cn

[Q76] 按天统计
来源：http://uka.birdmap.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sqc.tarul.cn

[Q77] 时间加减
来源：http://zvc.iojbl.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eah.meibo888.top

[Q78] 当前时间
来源：http://mps.nwbrower.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lby.vqdsnc.cn

[Q79] 字符串拼接
来源：http://xrc.yueranfly.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lbi.ydjk.org.cn

[Q80] 字符串截取
来源：http://dcl.cucudq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kkg.zycfv.cn

[Q81] 字符串替换
来源：http://shf.zhiwuduotai.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ags.gaohongyu789.top

[Q82] 字符长度与字节长度
来源：http://zem.tanke756.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ekd.vqdsnc.cn

[Q83] 大小写转换
来源：http://hhw.xinyue.icu

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pwa.tianlin.xyz

[Q84] 去除首尾空格
来源：http://nca.sweek.top

SELECT TRIM(name) FROM users;
来源：http://lwq.jinqigfzy.top

[Q85] 数值取整
来源：http://hli.quarkkingdee.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qnv.daxiang520.top

[Q86] 读取 JSON 字段
来源：http://vwy.ydjk.org.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cfk.dianchejie.cn

[Q87] JSON 字段做条件
来源：http://tgp.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hnv.cheryme.top

[Q88] 行转列（条件聚合）
来源：http://yqy.tian-w.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kgv.fktsv.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mnp.havefunace.top

[Q89] 判断表是否存在
来源：http://drn.chenlongwang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wxe.guowangkeji.top

[Q90] 生成序号列
来源：http://ftn.cqqwz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://acp.gaohongyu789.top

================================================================================
来源：http://apy.fehbvm.com

R. Bash 专题
来源：http://vum.tanke756.top

================================================================================
来源：http://jju.aizwys.cn

[R01] shebang 与严格模式
来源：http://hcq.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://xvx.vehdjk.com

set -euo pipefail
来源：http://pgp.redwolf501.top

[R02] 变量赋值与使用
来源：http://fll.yj20258888.top

name="Tom"; echo "$name"
来源：http://nuh.ppjwa.cn

[R03] 只读变量
来源：http://ycw.yj20258.top

readonly PI=3.14
来源：http://wyt.zdbjq.cn

[R04] 位置参数
来源：http://hwz.kuanghao11.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://npc.ybcxt.top

[R05] 参数默认值
来源：http://tln.jianghu66.top

name="${1:-default}"
来源：http://zkt.cqqwz.cn

[R06] 判断命令是否存在
来源：http://agc.guannengcc.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mjd.wangshuangyany.cn

[R07] if 判断文件
来源：http://smk.zdbjq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hlg.tarul.cn

[R08] 数值比较
来源：http://mlo.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cvo.havefunace.top

[R09] 字符串比较
来源：http://wrj.vehdjk.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qlm.shuidangran.top

[R10] 正则匹配
来源：http://dmx.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fuq.guannengcc.top

[R11] case 多分支
来源：http://tdz.sysykeji.top

case "$1" in
来源：http://tru.sysykeji.top

start) echo "启动" ;;
来源：http://xyp.jinqigfzy.top

stop)  echo "停止" ;;
来源：http://cok.hnxiangtu.top

*)     echo "未知命令" ;;
来源：http://rjj.ppjwa.cn

esac
来源：http://ons.guowangkeji.top

[R12] for 遍历文件
来源：http://mwq.cheryme.top

for f in *.txt; do echo "$f"; done
来源：http://dfw.ehwqpu.com

[R13] for 计数循环
来源：http://yjv.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://how.gotoacloud.top

[R14] C 风格 for
来源：http://jpi.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bfi.wangshuangyany.cn

[R15] while 逐行读文件
来源：http://aua.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://adi.jinqigfzy.top

[R16] until 等待条件
来源：http://qea.hammf.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kit.daxiang520.top

[R17] 数组定义与取值
来源：http://ygv.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://tfx.redwolf501.top

[R18] 遍历数组
来源：http://ptk.yj202588.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uoz.cucudq.cn

[R19] 数组长度
来源：http://mti.fktsv.cn

echo "${#arr[@]}"
来源：http://tvi.haohaochexian.top

[R20] 关联数组（字典）
来源：http://vuj.bbcook.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wmq.c1oappe.top

[R21] 字符串长度
来源：http://bxv.yonumen.top

echo "${#s}"
来源：http://yco.bbcook.cn

[R22] 截取子串
来源：http://dmz.redwolf501.top

echo "${s:0:5}"
来源：http://qiv.zdqjudy.top

[R23] 字符串替换
来源：http://pho.andypj.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mki.ppjwa.cn

[R24] 大小写转换
来源：http://lug.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://wxs.sysykeji.top

[R25] 去后缀 / 去前缀
来源：http://nmf.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zmn.fehbvm.com

[R26] 命令替换
来源：http://ckx.zhongyouzk.top

now=$(date +%F); echo "$now"
来源：http://rbz.sysykeji.top

[R27] 算术展开
来源：http://bjo.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://fmk.zdbjq.cn

[R28] 浮点运算
来源：http://ivt.hongshengwenyu.top

echo "scale=2; 10/3" | bc
来源：http://dua.cdnleiting.top

[R29] 定义函数
来源：http://bpz.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nzv.hnqzz.top

[R30] 函数返回状态码
来源：http://eqy.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://foz.hfpthk.cn

[R31] 局部变量
来源：http://pbx.sysykeji.top

f() { local x=1; echo "$x"; }
来源：http://nql.dashuyun.cn

[R32] 参数个数校验
来源：http://jbp.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fps.zhijiandao.cn

[R33] 捕获错误并提示行号
来源：http://jet.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cop.hysaishi.cn

[R34] 退出时清理
来源：http://udu.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://emq.ydjk.org.cn

[R35] 后台执行并等待
来源：http://lzy.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pcu.ydzc1.top

[R36] 并发执行多个任务
来源：http://nvo.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dri.yueranfly.top

[R37] 把输出赋给变量
来源：http://mxp.xingfuxueyuan.xyz

files=$(ls -1)
来源：http://syo.wangdashe.top

[R38] 管道串联
来源：http://gks.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://otm.ydjk.org.cn

[R39] 重定向标准输出与错误
来源：http://svf.pycfn.com

cmd > out.log 2>&1
来源：http://kbz.tarul.cn

[R40] 追加写日志
来源：http://kzs.ppjwa.cn

echo "log" >> out.log
来源：http://wxr.tian-w.cn

[R41] 丢弃输出
来源：http://mbw.0kj1m.cn

cmd >/dev/null 2>&1
来源：http://gru.gzhubu.top

[R42] 输入重定向
来源：http://xuk.guowangkeji.top

wc -l < a.txt
来源：http://wtt.yfazqb.com

[R43] 按名字查找文件
来源：http://dze.yj202588.top

find . -name "*.log" -type f
来源：http://imr.yj202588.top

[R44] 按修改时间查找
来源：http://ehj.hfpthk.cn

find . -mtime -7 -type f
来源：http://bbs.zdqjudy.top

[R45] 批量删除
来源：http://mlr.meibo888.top

find . -name "*.tmp" -delete
来源：http://kiv.dashuyun.cn

[R46] 递归替换文件内容
来源：http://geq.kuanghao11.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ssn.feifeiyinyue.top

[R47] sed 单行替换
来源：http://qca.0kj1m.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dsw.gzhubu.top

[R48] awk 取指定列
来源：http://bbt.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://ljx.fengsongda.top

[R49] awk 带条件
来源：http://auj.tanke756.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iyd.meibo888.top

[R50] awk 求和
来源：http://wyh.hongshengwenyu.top

awk '{s += $2} END {print s}' a.txt
来源：http://won.jlsjyb.cn

[R51] 排序去重取前几
来源：http://dtv.xziqi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hne.nanxuanxn.top

[R52] 统计行数
来源：http://hbp.aizwys.cn

wc -l a.txt
来源：http://xkq.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://tjz.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iea.jlsjyb.cn

[R54] 比较两个文件
来源：http://igl.yj20258888.top

diff a.txt b.txt
来源：http://oue.shuidangran.top

[R55] 压缩与解压
来源：http://szr.daria6918.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tzj.ydzc1.top

[R56] 远程拷贝
来源：http://trm.hywenlv.cn

scp file user@host:/path/
来源：http://zcx.jqgfzy.top

[R57] 远程执行命令
来源：http://tlc.yfazqb.com

ssh user@host 'uptime'
来源：http://tqk.chenjidiqi.icu

[R58] 下载文件
来源：http://wdk.redwolf501.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kdp.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://gyq.sxryk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mob.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://xxu.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://imq.xinyue.icu

[R61] 磁盘占用
来源：http://qpo.jqgufenzy.top

df -h;  du -sh *
来源：http://prl.xingfuxueyuan.xyz

[R62] 找最占空间的文件
来源：http://jls.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://nmg.9152youxi.cn

[R63] 内存与进程
来源：http://fls.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://gcc.birdmap.top

[R64] 结束进程
来源：http://edp.zdqjudy.top

kill -9 $(pgrep -f app.py)
来源：http://mue.guowangkeji.top

[R65] 查看端口占用
来源：http://tzw.wangdashe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hwi.yuanzhike.top

[R66] 定时任务
来源：http://ooo.bjfxy.top

crontab -e;  crontab -l
来源：http://reo.fengsongda.top

[R67] 生成随机十六进制串
来源：http://pil.sweek.top

openssl rand -hex 16
来源：http://hvp.hammf.cn

[R68] 计算文件校验值
来源：http://uaj.yanxiufei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hrw.ctjpmb.com

[R69] 生成随机密码
来源：http://klg.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://cev.epnwcf.com

[R70] 时间戳与互转
来源：http://its.aizwys.cn

date +%s;  date -d @1700000000
来源：http://nki.svipenyu.cn

[R71] 日期格式化
来源：http://oqg.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://huc.52xcode.cn

[R72] 等待端口就绪
来源：http://crv.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hmw.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://gtd.pycfn.com

split -l 1000 big.log part_
来源：http://wpb.yueranfly.top

[R74] 批量重命名
来源：http://loj.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ykv.chenlongwang.top

[R75] 导出环境变量
来源：http://btn.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://soy.zhengqikj.top

[R76] 使用临时文件
来源：http://ncl.ydzc1.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://luy.yj202588.top

[R77] 读取用户输入
来源：http://ixa.xziqi.cn

read -rp "请输入: " ans
来源：http://ysj.xuanzx.com

[R78] 交互式菜单
来源：http://dqh.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ddh.redwolf501.top

[R79] 解析命令行选项
来源：http://hlc.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dqd.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://svh.vehdjk.com

time ./run.sh
来源：http://oyr.birdmap.top

================================================================================
来源：http://qvs.xinyue.icu

S. C / C++ 专题
来源：http://paj.uphjek.com

================================================================================
来源：http://sip.jyoumei.cn

[S01] C：Hello World
来源：http://rgt.ydjk.org.cn

#include <stdio.h>
来源：http://xqn.yuxming.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hyx.nwbrower.top

[S02] C：变量与格式化输出
来源：http://hci.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://fcw.cheryme.top

[S03] C：读入整数
来源：http://imn.jianghu66.top

int x; scanf("%d", &x);
来源：http://qdr.wangshuangyany.cn

[S04] C：字符串复制
来源：http://try.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://puy.zhengqikj.top

[S05] C：字符串长度
来源：http://lqu.kuanghao11.cn

strlen(s)
来源：http://cqw.uphjek.com

[S06] C：字符串比较
来源：http://rac.ydzc1.top

strcmp(a, b) == 0
来源：http://akm.jiagoushi.top

[S07] C：数组遍历求和
来源：http://hvx.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hbv.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://fqe.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ylb.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://dgb.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ycz.jiagoushi.top

[S10] C：指针与解引用
来源：http://lsr.jinqigufen.top

int *p = &a;  *p = 5;
来源：http://est.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://sux.daria6918.cn

FILE *f = fopen("a.txt", "r");
来源：http://cjy.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mpn.gotoacloud.top

fclose(f);
来源：http://woe.ivvv.top

[S12] C：写文件
来源：http://ktx.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kzq.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://uwh.guannengcc.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blr.wangshuangyany.cn

[S14] C：枚举
来源：http://ute.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://aye.ybcxt.top

[S15] C：类型转换
来源：http://ovh.hcnkem.com

(double) a / b
来源：http://hzd.ydjk.org.cn

[S16] C：位操作置位
来源：http://nee.tianlin.xyz

x |= (1 << 3);
来源：http://owm.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://vsp.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bba.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://voq.chenzaomai.com

int main(int argc, char **argv)
来源：http://upl.9152youxi.cn

[S19] C：快速排序
来源：http://sbl.vehdjk.com

qsort(a, n, sizeof(int), cmp);
来源：http://lrg.nanxuanxn.top

[S20] C：二分查找
来源：http://yze.cdnleiting.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zup.wangshuangyany.cn

[S21] C：字符类别判断
来源：http://btk.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bxt.yj20258888.top

[S22] C：字符串转数字
来源：http://eou.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cml.feifeiyinyue.top

[S23] C：随机数
来源：http://ysz.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ysx.zycfv.cn

[S24] C：获取本地时间
来源：http://blb.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://buq.epnwcf.com

[S25] C：内存拷贝
来源：http://apz.ydzc1.top

memcpy(dst, src, n);
来源：http://wnr.jiagoushi.top

[S26] C：内存清零
来源：http://hxh.fktsv.cn

memset(a, 0, sizeof a);
来源：http://uud.ehwqpu.com

[S27] C：定义常量
来源：http://uvm.daxiang520.top

const double PI = 3.14159;
来源：http://cna.fehbvm.com

[S28] C：静态变量
来源：http://juk.tarul.cn

static int counter = 0;
来源：http://swq.pengpengdd.cyou

[S29] C：变参函数
来源：http://vcd.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nbq.zhixingplan.top

[S30] C：头文件保护
来源：http://ser.gaohongyu789.top

#ifndef X_H
来源：http://gzm.jinqigufen.top

#define X_H
来源：http://vmo.dashuyun.cn

#endif
来源：http://xez.daria6918.cn

[S31] C++：Hello World
来源：http://zfq.ybcxt.top

#include <iostream>
来源：http://fua.fanxiaobao.xyz

int main() { std::cout << "Hello\n"; }
来源：http://fpa.fzhhl.top

[S32] C++：字符串
来源：http://mim.tarul.cn

std::string s = "hi";  s += "!";
来源：http://dpv.hammf.cn

[S33] C++：vector 增删
来源：http://rul.andypj.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kxv.yj20258888.top

[S34] C++：遍历 vector
来源：http://ugy.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://zck.redwolf501.top

[S35] C++：map
来源：http://osn.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wpw.hysaishi.cn

[S36] C++：unordered_map
来源：http://tue.ydzc1.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ymy.hywenlv.cn

[S37] C++：set
来源：http://vjc.aibaodan.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iju.fanxiaobao.xyz

[S38] C++：排序
来源：http://qko.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://xdc.guowangkeji.top

[S39] C++：自定义比较器排序
来源：http://tqa.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uix.sweek.top

[S40] C++：查找元素
来源：http://uzo.zdqjudy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ivs.aizwys.cn

[S41] C++：类与构造函数
来源：http://vau.sjlbkw.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mrw.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://rwj.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://fcv.guowangkeji.top


<!-- 参考信息 -->