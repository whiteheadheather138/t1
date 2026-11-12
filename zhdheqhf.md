代发 wailian999

[Q65] 回滚事务
来源：http://ogj.redwolf501.top

ROLLBACK;
来源：http://uda.hammf.cn

[Q66] 行锁查询
来源：http://bis.hysaishi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://msq.iojbl.cn

[Q67] 设置隔离级别
来源：http://uzw.zhaomingkeji.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fyn.guowangkeji.top

[Q68] 保存点
来源：http://fld.zhixingplan.top

SAVEPOINT sp1;
来源：http://njn.tanke756.top

ROLLBACK TO sp1;
来源：http://obb.daria6918.cn

[Q69] 查看执行计划
来源：http://jsk.hywenlv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ksq.xuetiantiany.cn

[Q70] 更新统计信息
来源：http://ptw.dashuyun.cn

ANALYZE TABLE users;
来源：http://kej.jqgufenzy.top

[Q71] 查看建表语句
来源：http://xdb.ydjk.org.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nbj.nanxuanxn.top

[Q72] 查看索引
来源：http://hwi.bjfxy.top

SHOW INDEX FROM users;
来源：http://iwy.xingfuxueyuan.xyz

[Q73] 查看表状态
来源：http://dra.cqqwz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://upv.cqqwz.cn

[Q74] 强制使用索引
来源：http://exy.sysykeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ppw.hnqzz.top

[Q75] 日期格式化
来源：http://wdi.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aoe.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tau.yangfankeji.com

[Q76] 按天统计
来源：http://rhl.yonumen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hna.shzxlz.cn

[Q77] 时间加减
来源：http://dqs.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kgr.fzhhl.top

[Q78] 当前时间
来源：http://wgh.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://weh.shzxlz.cn

[Q79] 字符串拼接
来源：http://cmp.fanxiaobao.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pxu.jqgufenzy.top

[Q80] 字符串截取
来源：http://kxl.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dik.havefunace.top

[Q81] 字符串替换
来源：http://zfy.jianghu66.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://phg.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://txm.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wgg.birdmap.top

[Q83] 大小写转换
来源：http://sdm.vqdsnc.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://efa.ctjpmb.com

[Q84] 去除首尾空格
来源：http://jzk.zdbjq.cn

SELECT TRIM(name) FROM users;
来源：http://vby.yuanzhike.top

[Q85] 数值取整
来源：http://rcq.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://unt.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://lyx.jiagoushi.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rhj.zhixingplan.top

[Q87] JSON 字段做条件
来源：http://cnt.yj20258888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ygx.gzhubu.top

[Q88] 行转列（条件聚合）
来源：http://hga.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pwm.gogol.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nak.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://kqz.hysaishi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ynb.xuanzx.com

[Q90] 生成序号列
来源：http://fme.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sat.dianchejie.cn

================================================================================
来源：http://bvj.0kj1m.cn

R. Bash 专题
来源：http://qap.guannengcc.top

================================================================================
来源：http://nby.jlsjyb.cn

[R01] shebang 与严格模式
来源：http://zxl.52xcode.cn

#!/usr/bin/env bash
来源：http://tsg.ctjpmb.com

set -euo pipefail
来源：http://jub.haohaochexian.top

[R02] 变量赋值与使用
来源：http://ccq.haohaochexian.top

name="Tom"; echo "$name"
来源：http://vsy.tarul.cn

[R03] 只读变量
来源：http://tao.shanyushiyangkeji.top

readonly PI=3.14
来源：http://cyi.shzxlz.cn

[R04] 位置参数
来源：http://psz.zdqjudy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rah.jqgufenzy.top

[R05] 参数默认值
来源：http://etk.yuanzhike.top

name="${1:-default}"
来源：http://uyi.tian-w.cn

[R06] 判断命令是否存在
来源：http://dpx.jqgfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ygp.havefunace.top

[R07] if 判断文件
来源：http://hjy.shanyushiyangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qwa.nanxuanxn.top

[R08] 数值比较
来源：http://lkj.jinqigfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://xmb.hnqzz.top

[R09] 字符串比较
来源：http://lbf.zhongyouzk.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mzs.gaohongyu789.top

[R10] 正则匹配
来源：http://nlh.chenjidiqi.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zjr.redwolf501.top

[R11] case 多分支
来源：http://dvu.jinyuanbaomall.cn

case "$1" in
来源：http://qdo.zhongyouzk.top

start) echo "启动" ;;
来源：http://rpm.xziqi.cn

stop)  echo "停止" ;;
来源：http://wrd.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://jwr.sjlbkw.cn

esac
来源：http://eqo.haohaochexian.top

[R12] for 遍历文件
来源：http://ovl.0kj1m.cn

for f in *.txt; do echo "$f"; done
来源：http://mlr.cqqwz.cn

[R13] for 计数循环
来源：http://ptc.jinqigfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://tgq.zhijiandao.cn

[R14] C 风格 for
来源：http://mtt.52xcode.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tzg.bjfxy.top

[R15] while 逐行读文件
来源：http://dhv.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xoi.dianchejie.cn

[R16] until 等待条件
来源：http://fpj.haohaochexian.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ejx.jinqigfzy.top

[R17] 数组定义与取值
来源：http://lyl.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://gjo.xinyue.icu

[R18] 遍历数组
来源：http://udc.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gan.tanke756.top

[R19] 数组长度
来源：http://kwj.daxiang520.top

echo "${#arr[@]}"
来源：http://qin.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://rid.zhiwuduotai.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ucd.9152youxi.cn

[R21] 字符串长度
来源：http://iig.ivvv.top

echo "${#s}"
来源：http://ksi.tian-w.cn

[R22] 截取子串
来源：http://hvx.pengpengdd.cyou

echo "${s:0:5}"
来源：http://fpo.tarul.cn

[R23] 字符串替换
来源：http://lfx.jiagoushi.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://evh.bjfxy.top

[R24] 大小写转换
来源：http://mvs.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://lmx.dashuyun.cn

[R25] 去后缀 / 去前缀
来源：http://jbe.zycfv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vbj.ydzc1.top

[R26] 命令替换
来源：http://eps.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://ena.yongpay.top

[R27] 算术展开
来源：http://vzr.zdqjudy.top

echo $((1 + 2 * 3))
来源：http://rcx.jinyuanbaomall.cn

[R28] 浮点运算
来源：http://goj.cheryme.top

echo "scale=2; 10/3" | bc
来源：http://oak.ydzc1.top

[R29] 定义函数
来源：http://uoe.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eno.dashuyun.cn

[R30] 函数返回状态码
来源：http://sna.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://qet.haohaochexian.top

[R31] 局部变量
来源：http://dzl.sxryk.cn

f() { local x=1; echo "$x"; }
来源：http://oeo.ctjpmb.com

[R32] 参数个数校验
来源：http://rmg.tian-w.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fcb.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://ner.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pzv.yangfankeji.com

[R34] 退出时清理
来源：http://nax.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://luq.zhaomingkeji.xyz

[R35] 后台执行并等待
来源：http://alw.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kqe.guowangkeji.top

[R36] 并发执行多个任务
来源：http://lem.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gzl.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://dak.hnxiangtu.top

files=$(ls -1)
来源：http://osw.cheryme.top

[R38] 管道串联
来源：http://zwq.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://pkq.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://umb.gogol.net.cn

cmd > out.log 2>&1
来源：http://irr.nanxuanxn.top

[R40] 追加写日志
来源：http://hdc.zdbjq.cn

echo "log" >> out.log
来源：http://rce.mhx1999.top

[R41] 丢弃输出
来源：http://kqr.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://rlh.tarul.cn

[R42] 输入重定向
来源：http://qto.hcnkem.com

wc -l < a.txt
来源：http://aqh.zdbjq.cn

[R43] 按名字查找文件
来源：http://ijc.ehwqpu.com

find . -name "*.log" -type f
来源：http://cyj.dianchejie.cn

[R44] 按修改时间查找
来源：http://fii.aibaodan.cn

find . -mtime -7 -type f
来源：http://gam.tarul.cn

[R45] 批量删除
来源：http://via.daxiang520.top

find . -name "*.tmp" -delete
来源：http://ixj.hesvh.cn

[R46] 递归替换文件内容
来源：http://vxj.yanxiufei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rir.shzxlz.cn

[R47] sed 单行替换
来源：http://cbg.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://hsk.316326.xyz

[R48] awk 取指定列
来源：http://erh.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://pou.yongpay.top

[R49] awk 带条件
来源：http://crt.c1oappe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qpo.gotoacloud.top

[R50] awk 求和
来源：http://dof.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ohl.ybcxt.top

[R51] 排序去重取前几
来源：http://rlo.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pej.zhoulong.xyz

[R52] 统计行数
来源：http://ewd.svipenyu.cn

wc -l a.txt
来源：http://qeq.shangyingyoupin.top

[R53] 查看文件头与实时尾
来源：http://meq.jinqigufen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tlh.tanke756.top

[R54] 比较两个文件
来源：http://qqc.vehdjk.com

diff a.txt b.txt
来源：http://oaz.kuanghao11.cn

[R55] 压缩与解压
来源：http://jvt.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pds.svipenyu.cn

[R56] 远程拷贝
来源：http://phr.gogol.net.cn

scp file user@host:/path/
来源：http://usl.pengpengdd.cyou

[R57] 远程执行命令
来源：http://qkg.jianghu66.top

ssh user@host 'uptime'
来源：http://jbr.svipenyu.cn

[R58] 下载文件
来源：http://bks.zdbjq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dlt.aizwys.cn

[R59] 发 POST JSON
来源：http://dyj.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cgm.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://xbk.tanke756.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gqu.yfazqb.com

[R61] 磁盘占用
来源：http://sud.yj20258.top

df -h;  du -sh *
来源：http://tnh.nanxinkj.top

[R62] 找最占空间的文件
来源：http://xbi.jinyuanbaomall.cn

du -ah . | sort -rh | head -10
来源：http://lbn.guannengcc.top

[R63] 内存与进程
来源：http://rea.yangfankeji.com

free -h;  ps aux | grep nginx
来源：http://lox.iojbl.cn

[R64] 结束进程
来源：http://rai.quarkkingdee.top

kill -9 $(pgrep -f app.py)
来源：http://cnb.hywenlv.cn

[R65] 查看端口占用
来源：http://vei.gogol.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hfn.andypj.xyz

[R66] 定时任务
来源：http://ztb.iojbl.cn

crontab -e;  crontab -l
来源：http://ngq.hesvh.cn

[R67] 生成随机十六进制串
来源：http://etq.epnwcf.com

openssl rand -hex 16
来源：http://jcy.cqqwz.cn

[R68] 计算文件校验值
来源：http://nia.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://uwi.snrcjt.cn

[R69] 生成随机密码
来源：http://qnm.shanyushiyangkeji.top

head -c 16 /dev/urandom | base64
来源：http://ogf.zhoulong.xyz

[R70] 时间戳与互转
来源：http://hky.hesvh.cn

date +%s;  date -d @1700000000
来源：http://jwr.jqgfzy.top

[R71] 日期格式化
来源：http://wns.sxryk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bxi.yuxming.cn

[R72] 等待端口就绪
来源：http://vkf.dianchejie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oup.sysykeji.top

[R73] 分割大日志
来源：http://spl.gaohongyu789.top

split -l 1000 big.log part_
来源：http://iyt.fehbvm.com

[R74] 批量重命名
来源：http://bzh.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yav.yonumen.top

[R75] 导出环境变量
来源：http://grk.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://vnb.sxryk.cn

[R76] 使用临时文件
来源：http://ijn.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mfy.cucudq.cn

[R77] 读取用户输入
来源：http://yvx.yonumen.top

read -rp "请输入: " ans
来源：http://heg.zhaomingkeji.xyz

[R78] 交互式菜单
来源：http://xjq.jiagoushi.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jeb.tarul.cn

[R79] 解析命令行选项
来源：http://bai.sufxvd.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dku.yj202588.top

[R80] 查看脚本执行耗时
来源：http://whz.ppjwa.cn

time ./run.sh
来源：http://pie.nanxinkj.top

================================================================================
来源：http://rrh.9152youxi.cn

S. C / C++ 专题
来源：http://yqv.xuanzx.com

================================================================================
来源：http://kef.chenzaomai.com

[S01] C：Hello World
来源：http://ygd.redwolf501.top

#include <stdio.h>
来源：http://ldo.guowangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jhp.fzhhl.top

[S02] C：变量与格式化输出
来源：http://nga.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://tok.nanxinkj.top

[S03] C：读入整数
来源：http://idq.chenlongwang.top

int x; scanf("%d", &x);
来源：http://zjb.pycfn.com

[S04] C：字符串复制
来源：http://hqb.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://kww.uphjek.com

[S05] C：字符串长度
来源：http://lcm.shanyushiyangtech.top

strlen(s)
来源：http://rkr.ydjk.org.cn

[S06] C：字符串比较
来源：http://quv.hnqzz.top

strcmp(a, b) == 0
来源：http://cej.yvedp.cn

[S07] C：数组遍历求和
来源：http://vfn.tanke756.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lch.sweek.top

[S08] C：动态内存分配与释放
来源：http://jnr.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nqy.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://hxs.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gya.sweek.top

[S10] C：指针与解引用
来源：http://zme.yuxming.cn

int *p = &a;  *p = 5;
来源：http://qbd.redwolf501.top

[S11] C：逐行读文件
来源：http://kll.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://voe.jianghu66.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bmz.gzhubu.top

fclose(f);
来源：http://zty.shanyushiyangkeji.top

[S12] C：写文件
来源：http://aro.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hbx.guowangkeji.top

[S13] C：宏定义
来源：http://okt.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://owt.pengpengdd.cyou

[S14] C：枚举
来源：http://vhx.yj202588.top

enum Color { RED, GREEN, BLUE };
来源：http://svx.sweek.top

[S15] C：类型转换
来源：http://cpd.cucudq.cn

(double) a / b
来源：http://vkp.ydzc1.top

[S16] C：位操作置位
来源：http://enm.epnwcf.com

x |= (1 << 3);
来源：http://xkh.ctjpmb.com

[S17] C：安全拼接字符串
来源：http://vtw.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ndm.zhijiandao.cn

[S18] C：命令行参数
来源：http://wfn.zhengqikj.top

int main(int argc, char **argv)
来源：http://xns.nanxuanxn.top

[S19] C：快速排序
来源：http://gvr.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://aiv.uphjek.com

[S20] C：二分查找
来源：http://uec.ywan-chungtsiang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://thj.tian-w.cn

[S21] C：字符类别判断
来源：http://rxj.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fee.fzhhl.top

[S22] C：字符串转数字
来源：http://vtv.shuidangran.top

atoi("42");  strtod("3.14", NULL);
来源：http://kbe.jqgfzy.top

[S23] C：随机数
来源：http://xsw.feifeiyinyue.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fmi.9152youxi.cn

[S24] C：获取本地时间
来源：http://svv.zdbjq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lxc.aizwys.cn

[S25] C：内存拷贝
来源：http://zek.fengsongda.top

memcpy(dst, src, n);
来源：http://jtx.tianlin.xyz

[S26] C：内存清零
来源：http://ofy.daria6918.cn

memset(a, 0, sizeof a);
来源：http://eli.jyoumei.cn

[S27] C：定义常量
来源：http://ruf.fengsongda.top

const double PI = 3.14159;
来源：http://okf.jinghuilouyu.cn

[S28] C：静态变量
来源：http://bqe.hcnkem.com

static int counter = 0;
来源：http://gor.ybcxt.top

[S29] C：变参函数
来源：http://dad.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://evs.52xcode.cn

[S30] C：头文件保护
来源：http://qgz.hongshengwenyu.top

#ifndef X_H
来源：http://xid.shanyushiyangkeji.top

#define X_H
来源：http://evu.cqqwz.cn

#endif
来源：http://hwa.vehdjk.com

[S31] C++：Hello World
来源：http://wad.svipenyu.cn

#include <iostream>
来源：http://sqq.xziqi.cn

int main() { std::cout << "Hello\n"; }
来源：http://rqs.jqgufenzy.top

[S32] C++：字符串
来源：http://ple.yj20258.top

std::string s = "hi";  s += "!";
来源：http://gjp.xinyue.icu

[S33] C++：vector 增删
来源：http://yzd.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tyt.hysaishi.cn

[S34] C++：遍历 vector
来源：http://izp.mhx1999.top

for (auto &x : v) { std::cout << x; }
来源：http://jju.hysaishi.cn


<!-- 参考信息 -->