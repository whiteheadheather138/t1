代发 wailian999

[Q63] 开启事务
来源：http://hle.ywan-chungtsiang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vsq.tian-w.cn

[Q64] 提交事务
来源：http://wyp.jinyuanbaomall.cn

COMMIT;
来源：http://iaj.jiagoushi.top

[Q65] 回滚事务
来源：http://dkh.yuxming.cn

ROLLBACK;
来源：http://iga.gzhubu.top

[Q66] 行锁查询
来源：http://ngt.mhx1999.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://drj.sjlbkw.cn

[Q67] 设置隔离级别
来源：http://jcu.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rxm.vehdjk.com

[Q68] 保存点
来源：http://hhj.yongpay.top

SAVEPOINT sp1;
来源：http://ixb.gotoacloud.top

ROLLBACK TO sp1;
来源：http://mft.52xcode.cn

[Q69] 查看执行计划
来源：http://uft.hcnkem.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tai.wangdashe.top

[Q70] 更新统计信息
来源：http://kui.aibaodan.cn

ANALYZE TABLE users;
来源：http://aie.yangfankeji.com

[Q71] 查看建表语句
来源：http://yjf.cashguo.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bbx.zycfv.cn

[Q72] 查看索引
来源：http://plq.yangfankeji.com

SHOW INDEX FROM users;
来源：http://wzj.xylfe.cn

[Q73] 查看表状态
来源：http://msq.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://itm.zdbjq.cn

[Q74] 强制使用索引
来源：http://jmz.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://npw.xingfuxueyuan.xyz

[Q75] 日期格式化
来源：http://feg.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zfn.gaohongyu789.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vgq.kuanghao11.cn

[Q76] 按天统计
来源：http://ypb.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dyz.c1oappe.top

[Q77] 时间加减
来源：http://qyh.xingfuxueyuan.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iqj.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://eqp.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xay.wangdashe.top

[Q79] 字符串拼接
来源：http://bff.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vww.birdmap.top

[Q80] 字符串截取
来源：http://emp.svipenyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wyh.shanyushiyangkeji.top

[Q81] 字符串替换
来源：http://fwt.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gzh.zhixingplan.top

[Q82] 字符长度与字节长度
来源：http://zbt.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rrn.xylfe.cn

[Q83] 大小写转换
来源：http://rnq.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fgt.svipenyu.cn

[Q84] 去除首尾空格
来源：http://zyk.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://uaw.haohaochexian.top

[Q85] 数值取整
来源：http://zlc.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fjm.svipenyu.cn

[Q86] 读取 JSON 字段
来源：http://llu.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pqd.pycfn.com

[Q87] JSON 字段做条件
来源：http://gmd.jianghu66.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jmq.epnwcf.com

[Q88] 行转列（条件聚合）
来源：http://zhb.smart0.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zqj.vehdjk.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vgi.jinyuanbaomall.cn

[Q89] 判断表是否存在
来源：http://jbl.shangyingyoupin.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wam.iojbl.cn

[Q90] 生成序号列
来源：http://eyu.cdnleiting.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jhz.jqgufenzy.top

================================================================================
来源：http://xzr.jyoumei.cn

R. Bash 专题
来源：http://cgp.ivvv.top

================================================================================
来源：http://hwk.zdbjq.cn

[R01] shebang 与严格模式
来源：http://mqz.epnwcf.com

#!/usr/bin/env bash
来源：http://nst.hywenlv.cn

set -euo pipefail
来源：http://sbu.wangdashe.top

[R02] 变量赋值与使用
来源：http://sxx.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://pii.snrcjt.cn

[R03] 只读变量
来源：http://hpe.shuidangran.top

readonly PI=3.14
来源：http://kid.shanyushiyangtech.top

[R04] 位置参数
来源：http://vsl.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jga.ivvv.top

[R05] 参数默认值
来源：http://ule.tarul.cn

name="${1:-default}"
来源：http://mat.jyoumei.cn

[R06] 判断命令是否存在
来源：http://gbx.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://itq.zhoulong.xyz

[R07] if 判断文件
来源：http://pdr.sufxvd.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fyb.birdmap.top

[R08] 数值比较
来源：http://ycz.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://flr.ppjwa.cn

[R09] 字符串比较
来源：http://wtp.hnxiangtu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bfd.c1oappe.top

[R10] 正则匹配
来源：http://knc.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://usk.fengsongda.top

[R11] case 多分支
来源：http://gmu.xylfe.cn

case "$1" in
来源：http://foq.zhijiandao.cn

start) echo "启动" ;;
来源：http://wan.gzhubu.top

stop)  echo "停止" ;;
来源：http://cgz.jiagoushi.top

*)     echo "未知命令" ;;
来源：http://nbx.yueranfly.top

esac
来源：http://obf.tarul.cn

[R12] for 遍历文件
来源：http://ney.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://ukr.hammf.cn

[R13] for 计数循环
来源：http://lce.yueranfly.top

for i in {1..10}; do echo "$i"; done
来源：http://nju.gogol.net.cn

[R14] C 风格 for
来源：http://fzp.fzhhl.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jxu.wangshuangyany.cn

[R15] while 逐行读文件
来源：http://ldq.sweek.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sdl.9152youxi.cn

[R16] until 等待条件
来源：http://qwa.cheryme.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gmw.ppjwa.cn

[R17] 数组定义与取值
来源：http://kbf.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://gdt.havefunace.top

[R18] 遍历数组
来源：http://gfk.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sfq.jinqigfzy.top

[R19] 数组长度
来源：http://jnv.dianchejie.cn

echo "${#arr[@]}"
来源：http://iad.zhixingplan.top

[R20] 关联数组（字典）
来源：http://voy.jyoumei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://noz.zhongyouzk.top

[R21] 字符串长度
来源：http://smw.hongshengwenyu.top

echo "${#s}"
来源：http://ryf.guowangkeji.top

[R22] 截取子串
来源：http://nve.zhiwuduotai.top

echo "${s:0:5}"
来源：http://pzw.epnwcf.com

[R23] 字符串替换
来源：http://jbz.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vxx.yuxming.cn

[R24] 大小写转换
来源：http://mek.xuanzx.com

echo "${s^^}"; echo "${s,,}"
来源：http://apo.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://lzc.zhixingplan.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://aun.yvedp.cn

[R26] 命令替换
来源：http://xgc.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://obd.0kj1m.cn

[R27] 算术展开
来源：http://six.c1oappe.top

echo $((1 + 2 * 3))
来源：http://wpl.ydzc1.top

[R28] 浮点运算
来源：http://xhq.yanxiufei.cn

echo "scale=2; 10/3" | bc
来源：http://ptw.snrcjt.cn

[R29] 定义函数
来源：http://uij.xziqi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xtt.ctjpmb.com

[R30] 函数返回状态码
来源：http://ezf.quarkkingdee.top

f() { return 0; }; f || echo "失败了"
来源：http://gkm.shuidangran.top

[R31] 局部变量
来源：http://jqa.vehdjk.com

f() { local x=1; echo "$x"; }
来源：http://flk.epnwcf.com

[R32] 参数个数校验
来源：http://xub.nanxuanxn.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fkb.xuanzx.com

[R33] 捕获错误并提示行号
来源：http://ncp.hfpthk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dze.tanke756.top

[R34] 退出时清理
来源：http://esx.hongshengwenyu.top

trap 'rm -f "$tmp"' EXIT
来源：http://qmu.tanke756.top

[R35] 后台执行并等待
来源：http://qww.sweek.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jyl.mhx1999.top

[R36] 并发执行多个任务
来源：http://xwg.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vkn.hammf.cn

[R37] 把输出赋给变量
来源：http://vng.ppjwa.cn

files=$(ls -1)
来源：http://zqx.havefunace.top

[R38] 管道串联
来源：http://kkp.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://tck.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://fsi.aizwys.cn

cmd > out.log 2>&1
来源：http://itf.yj20258888.top

[R40] 追加写日志
来源：http://eyv.yanxiufei.cn

echo "log" >> out.log
来源：http://bca.zhaomingkeji.xyz

[R41] 丢弃输出
来源：http://kmg.nanxinkj.top

cmd >/dev/null 2>&1
来源：http://shh.jyoumei.cn

[R42] 输入重定向
来源：http://ciz.hcnkem.com

wc -l < a.txt
来源：http://pcc.shanyushiyangtech.top

[R43] 按名字查找文件
来源：http://jbq.daxiang520.top

find . -name "*.log" -type f
来源：http://gkp.ywan-chungtsiang.top

[R44] 按修改时间查找
来源：http://nhm.c1oappe.top

find . -mtime -7 -type f
来源：http://qpy.zhijiandao.cn

[R45] 批量删除
来源：http://kir.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://zwe.chenjidiqi.icu

[R46] 递归替换文件内容
来源：http://eqs.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gea.c1oappe.top

[R47] sed 单行替换
来源：http://cus.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://lrg.andypj.xyz

[R48] awk 取指定列
来源：http://tlw.cashguo.top

awk '{print $1, $3}' a.txt
来源：http://bfi.ctjpmb.com

[R49] awk 带条件
来源：http://kad.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://onj.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://rfv.jinyuanbaomall.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wsw.hongshengwenyu.top

[R51] 排序去重取前几
来源：http://iqq.zdqjudy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gru.pycfn.com

[R52] 统计行数
来源：http://hiu.ppjwa.cn

wc -l a.txt
来源：http://rpc.fzhhl.top

[R53] 查看文件头与实时尾
来源：http://gqp.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hmi.nanxuanxn.top

[R54] 比较两个文件
来源：http://wjd.gotoacloud.top

diff a.txt b.txt
来源：http://kum.fehbvm.com

[R55] 压缩与解压
来源：http://ncm.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lds.jqgufenzy.top

[R56] 远程拷贝
来源：http://dqv.birdmap.top

scp file user@host:/path/
来源：http://qjt.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://gqt.hysaishi.cn

ssh user@host 'uptime'
来源：http://osm.zhongyouzk.top

[R58] 下载文件
来源：http://oaz.aibaodan.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wsr.smart0.xyz

[R59] 发 POST JSON
来源：http://rrd.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://llr.jqgufenzy.top

[R60] 只看 HTTP 状态码
来源：http://jet.shanyushiyangtech.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wyz.jyoumei.cn

[R61] 磁盘占用
来源：http://pjb.fanxiaobao.xyz

df -h;  du -sh *
来源：http://fue.yfazqb.com

[R62] 找最占空间的文件
来源：http://bcc.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://nhr.jiagoushi.top

[R63] 内存与进程
来源：http://rer.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://mia.ppjwa.cn

[R64] 结束进程
来源：http://sbk.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://nqp.hongshengwenyu.top

[R65] 查看端口占用
来源：http://aet.kuanghao11.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xdh.pycfn.com

[R66] 定时任务
来源：http://yzl.pycfn.com

crontab -e;  crontab -l
来源：http://pdp.yj20258.top

[R67] 生成随机十六进制串
来源：http://qyk.gaohongyu789.top

openssl rand -hex 16
来源：http://yjs.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://lnq.yueranfly.top

sha256sum a.txt;  md5sum a.txt
来源：http://apl.sysykeji.top

[R69] 生成随机密码
来源：http://oyo.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://qji.yueranfly.top

[R70] 时间戳与互转
来源：http://qhk.fzhhl.top

date +%s;  date -d @1700000000
来源：http://qoz.jyoumei.cn

[R71] 日期格式化
来源：http://xga.dianchejie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qmo.jlsjyb.cn

[R72] 等待端口就绪
来源：http://nws.snrcjt.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fsd.yj202588.top

[R73] 分割大日志
来源：http://pgd.sweek.top

split -l 1000 big.log part_
来源：http://faw.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://vrx.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pcp.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://bor.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://yyz.yj20258888.top

[R76] 使用临时文件
来源：http://frn.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zbc.yuxming.cn

[R77] 读取用户输入
来源：http://xxs.ppjwa.cn

read -rp "请输入: " ans
来源：http://uud.gogol.net.cn

[R78] 交互式菜单
来源：http://snf.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://eci.zhoulong.xyz

[R79] 解析命令行选项
来源：http://gpa.dianchejie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://znn.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://blx.zhaomingkeji.xyz

time ./run.sh
来源：http://zfk.pengpengdd.cyou

================================================================================
来源：http://wka.jinqigfzy.top

S. C / C++ 专题
来源：http://onj.kuanghao11.cn

================================================================================
来源：http://hjd.tian-w.cn

[S01] C：Hello World
来源：http://ztm.yueranfly.top

#include <stdio.h>
来源：http://kck.ctjpmb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://vls.yj20258888.top

[S02] C：变量与格式化输出
来源：http://pvf.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://itu.vehdjk.com

[S03] C：读入整数
来源：http://nsw.jqgfzy.top

int x; scanf("%d", &x);
来源：http://mjf.zdbjq.cn

[S04] C：字符串复制
来源：http://nhe.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://mzs.havefunace.top

[S05] C：字符串长度
来源：http://sri.xingfuxueyuan.xyz

strlen(s)
来源：http://tkl.yonumen.top

[S06] C：字符串比较
来源：http://opz.pengpengdd.cyou

strcmp(a, b) == 0
来源：http://vgj.ywan-chungtsiang.top

[S07] C：数组遍历求和
来源：http://dcy.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://whu.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://mlh.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zfa.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://ydb.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zus.tianlin.xyz

[S10] C：指针与解引用
来源：http://qpa.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://jia.zdbjq.cn

[S11] C：逐行读文件
来源：http://fcl.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://cim.gaohongyu789.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bsm.chenlongwang.top

fclose(f);
来源：http://ilh.chenlongwang.top

[S12] C：写文件
来源：http://kuu.jqgfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ipy.9152youxi.cn

[S13] C：宏定义
来源：http://rsy.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ydx.chenlongwang.top

[S14] C：枚举
来源：http://ogb.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://mly.nwbrower.top

[S15] C：类型转换
来源：http://nkm.yanxiufei.cn

(double) a / b
来源：http://fgy.hysaishi.cn

[S16] C：位操作置位
来源：http://jcy.sweek.top

x |= (1 << 3);
来源：http://cvh.redwolf501.top

[S17] C：安全拼接字符串
来源：http://fhm.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hxf.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://uzt.zhixingplan.top

int main(int argc, char **argv)
来源：http://maa.dashuyun.cn

[S19] C：快速排序
来源：http://xoc.birdmap.top

qsort(a, n, sizeof(int), cmp);
来源：http://jvr.zhijiandao.cn

[S20] C：二分查找
来源：http://otd.mhx1999.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://roe.yj20258888.top

[S21] C：字符类别判断
来源：http://rya.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rlo.yongpay.top

[S22] C：字符串转数字
来源：http://uwm.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://nrb.yuxming.cn

[S23] C：随机数
来源：http://nht.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lwp.fengsongda.top

[S24] C：获取本地时间
来源：http://ita.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://shg.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://rmc.fktsv.cn

memcpy(dst, src, n);
来源：http://xxu.hcnkem.com

[S26] C：内存清零
来源：http://cok.iojbl.cn

memset(a, 0, sizeof a);
来源：http://byc.tianlin.xyz

[S27] C：定义常量
来源：http://twn.c1oappe.top

const double PI = 3.14159;
来源：http://vsl.jianghu66.top

[S28] C：静态变量
来源：http://vpk.hesvh.cn

static int counter = 0;
来源：http://pzr.sjlbkw.cn

[S29] C：变参函数
来源：http://zkd.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nyk.xinyue.icu

[S30] C：头文件保护
来源：http://nwg.yj202588.top

#ifndef X_H
来源：http://ozl.zhiwuduotai.top

#define X_H
来源：http://iru.jinqigufen.top

#endif
来源：http://fei.gotoacloud.top

[S31] C++：Hello World
来源：http://vjq.yuanzhike.top

#include <iostream>
来源：http://kze.zdqjudy.top

int main() { std::cout << "Hello\n"; }
来源：http://ftn.hammf.cn

[S32] C++：字符串
来源：http://ydn.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://lrp.cqqwz.cn


<!-- 参考信息 -->