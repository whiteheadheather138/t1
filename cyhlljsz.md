代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iha.zhoulong.xyz

[Q58] 累计求和
来源：http://qcv.bbcook.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rxo.fengsongda.top

[Q59] 分组内累计
来源：http://wwp.guowangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zwg.pengpengdd.cyou

[Q60] 取上一行 / 下一行
来源：http://ltz.ybcxt.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cyq.dianchejie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jep.xuetiantiany.cn

[Q61] 移动平均
来源：http://bvm.zhongyouzk.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qvh.hnqzz.top

[Q62] 分组占比
来源：http://qnp.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bzu.cqqwz.cn

[Q63] 开启事务
来源：http://cjn.shangyingyoupin.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fod.xuanzx.com

[Q64] 提交事务
来源：http://fmf.cdnleiting.top

COMMIT;
来源：http://phk.yj20258.top

[Q65] 回滚事务
来源：http://ggo.zhaomingkeji.xyz

ROLLBACK;
来源：http://nta.yuanzhike.top

[Q66] 行锁查询
来源：http://nve.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cpn.zdqjudy.top

[Q67] 设置隔离级别
来源：http://lbc.dashuyun.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ekm.andypj.xyz

[Q68] 保存点
来源：http://pyq.chenjidiqi.icu

SAVEPOINT sp1;
来源：http://ehh.epnwcf.com

ROLLBACK TO sp1;
来源：http://bri.epnwcf.com

[Q69] 查看执行计划
来源：http://jxc.tanke756.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ygq.ywan-chungtsiang.top

[Q70] 更新统计信息
来源：http://uso.smart0.xyz

ANALYZE TABLE users;
来源：http://lpq.yj20258.top

[Q71] 查看建表语句
来源：http://jhc.epnwcf.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iih.sysykeji.top

[Q72] 查看索引
来源：http://lhx.tianlin.xyz

SHOW INDEX FROM users;
来源：http://ups.fzhhl.top

[Q73] 查看表状态
来源：http://zyt.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pet.yuxming.cn

[Q74] 强制使用索引
来源：http://hwe.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ajh.havefunace.top

[Q75] 日期格式化
来源：http://ggf.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://byb.aibaodan.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hli.svipenyu.cn

[Q76] 按天统计
来源：http://uoh.tian-w.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xoz.jqgufenzy.top

[Q77] 时间加减
来源：http://tjc.jqgfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xgz.vehdjk.com

[Q78] 当前时间
来源：http://zfd.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://isa.shanyushiyangkeji.top

[Q79] 字符串拼接
来源：http://pjw.nanxuanxn.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yba.ppjwa.cn

[Q80] 字符串截取
来源：http://dok.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pzo.bjfxy.top

[Q81] 字符串替换
来源：http://dst.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zon.cashguo.top

[Q82] 字符长度与字节长度
来源：http://gfu.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mue.zdbjq.cn

[Q83] 大小写转换
来源：http://omx.aibaodan.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tgt.c1oappe.top

[Q84] 去除首尾空格
来源：http://drg.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://mru.fktsv.cn

[Q85] 数值取整
来源：http://gfj.haohaochexian.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mxx.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://rml.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jtl.havefunace.top

[Q87] JSON 字段做条件
来源：http://gdj.jyoumei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vfu.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://fup.shanyushiyangkeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zzf.chenzaomai.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nwt.uphjek.com

[Q89] 判断表是否存在
来源：http://wgh.ivvv.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uug.shuidangran.top

[Q90] 生成序号列
来源：http://wlk.yanxiufei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://imy.nwbrower.top

================================================================================
来源：http://sfw.xziqi.cn

R. Bash 专题
来源：http://uey.ivvv.top

================================================================================
来源：http://byq.vehdjk.com

[R01] shebang 与严格模式
来源：http://jsp.hysaishi.cn

#!/usr/bin/env bash
来源：http://uua.yongpay.top

set -euo pipefail
来源：http://dqw.yj202588.top

[R02] 变量赋值与使用
来源：http://jjb.tian-w.cn

name="Tom"; echo "$name"
来源：http://xpn.zhoulong.xyz

[R03] 只读变量
来源：http://hfb.dashuyun.cn

readonly PI=3.14
来源：http://xvv.guannengcc.top

[R04] 位置参数
来源：http://taw.cdnleiting.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uaf.shzxlz.cn

[R05] 参数默认值
来源：http://vvl.jinqigufen.top

name="${1:-default}"
来源：http://utf.bbcook.cn

[R06] 判断命令是否存在
来源：http://ssv.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pds.jinyuanbaomall.cn

[R07] if 判断文件
来源：http://hbr.haohaochexian.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cgo.yongpay.top

[R08] 数值比较
来源：http://ltv.gotoacloud.top

if (( a > b )); then echo "a 更大"; fi
来源：http://xup.zhaomingkeji.xyz

[R09] 字符串比较
来源：http://ohu.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wsu.vehdjk.com

[R10] 正则匹配
来源：http://cqc.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wwd.shanyushiyangkeji.top

[R11] case 多分支
来源：http://otf.shuidangran.top

case "$1" in
来源：http://snl.cashguo.top

start) echo "启动" ;;
来源：http://pzx.9152youxi.cn

stop)  echo "停止" ;;
来源：http://hnx.haohaochexian.top

*)     echo "未知命令" ;;
来源：http://yqd.xuanzx.com

esac
来源：http://wxh.wangshuangyany.cn

[R12] for 遍历文件
来源：http://han.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://pww.bbcook.cn

[R13] for 计数循环
来源：http://kke.pycfn.com

for i in {1..10}; do echo "$i"; done
来源：http://vfn.ywan-chungtsiang.top

[R14] C 风格 for
来源：http://ggw.jinyuanbaomall.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zvo.cashguo.top

[R15] while 逐行读文件
来源：http://fas.tianlin.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://glc.fengsongda.top

[R16] until 等待条件
来源：http://xgm.tianlin.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pwg.hnxiangtu.top

[R17] 数组定义与取值
来源：http://fpq.jinqigfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://yxl.feifeiyinyue.top

[R18] 遍历数组
来源：http://hqu.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jdd.c1oappe.top

[R19] 数组长度
来源：http://jjk.sjlbkw.cn

echo "${#arr[@]}"
来源：http://moy.nanxinkj.top

[R20] 关联数组（字典）
来源：http://mcn.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://noh.xuanzx.com

[R21] 字符串长度
来源：http://awq.hnqzz.top

echo "${#s}"
来源：http://uki.chenjidiqi.icu

[R22] 截取子串
来源：http://bly.tanke756.top

echo "${s:0:5}"
来源：http://ixn.gaohongyu789.top

[R23] 字符串替换
来源：http://ygr.cdnleiting.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qzt.zhijiandao.cn

[R24] 大小写转换
来源：http://eww.guannengcc.top

echo "${s^^}"; echo "${s,,}"
来源：http://foa.birdmap.top

[R25] 去后缀 / 去前缀
来源：http://bdx.kuanghao11.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dou.chenlongwang.top

[R26] 命令替换
来源：http://nrd.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://ylk.zhixingplan.top

[R27] 算术展开
来源：http://nnc.pycfn.com

echo $((1 + 2 * 3))
来源：http://bvv.sjlbkw.cn

[R28] 浮点运算
来源：http://zxu.nwbrower.top

echo "scale=2; 10/3" | bc
来源：http://nqk.epnwcf.com

[R29] 定义函数
来源：http://vqk.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://apj.sjlbkw.cn

[R30] 函数返回状态码
来源：http://gfo.ehwqpu.com

f() { return 0; }; f || echo "失败了"
来源：http://prs.jianghu66.top

[R31] 局部变量
来源：http://wjm.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://bql.wangdashe.top

[R32] 参数个数校验
来源：http://tao.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tae.jinghuilouyu.cn

[R33] 捕获错误并提示行号
来源：http://jck.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bad.cheryme.top

[R34] 退出时清理
来源：http://wsv.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://rgu.jqgfzy.top

[R35] 后台执行并等待
来源：http://vby.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jyw.meibo888.top

[R36] 并发执行多个任务
来源：http://jto.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ubx.gotoacloud.top

[R37] 把输出赋给变量
来源：http://ypk.tian-w.cn

files=$(ls -1)
来源：http://xtg.quarkkingdee.top

[R38] 管道串联
来源：http://gjy.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://hla.shuidangran.top

[R39] 重定向标准输出与错误
来源：http://yfu.yj20258.top

cmd > out.log 2>&1
来源：http://cfl.jqgufenzy.top

[R40] 追加写日志
来源：http://dfp.yuxming.cn

echo "log" >> out.log
来源：http://dmg.tanke756.top

[R41] 丢弃输出
来源：http://gas.snrcjt.cn

cmd >/dev/null 2>&1
来源：http://ojs.tian-w.cn

[R42] 输入重定向
来源：http://rla.yj202588.top

wc -l < a.txt
来源：http://ptg.iojbl.cn

[R43] 按名字查找文件
来源：http://vob.bbcook.cn

find . -name "*.log" -type f
来源：http://vga.wangshuangyany.cn

[R44] 按修改时间查找
来源：http://hwe.epnwcf.com

find . -mtime -7 -type f
来源：http://anj.c1oappe.top

[R45] 批量删除
来源：http://awa.snrcjt.cn

find . -name "*.tmp" -delete
来源：http://nog.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://tud.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://umm.vqdsnc.cn

[R47] sed 单行替换
来源：http://mjn.hcnkem.com

sed -i 's/foo/bar/g' a.txt
来源：http://lww.iojbl.cn

[R48] awk 取指定列
来源：http://axy.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://mfm.vqdsnc.cn

[R49] awk 带条件
来源：http://rjd.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nqp.fehbvm.com

[R50] awk 求和
来源：http://ttw.yuxming.cn

awk '{s += $2} END {print s}' a.txt
来源：http://miy.svipenyu.cn

[R51] 排序去重取前几
来源：http://zeu.jqgfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jrn.yueranfly.top

[R52] 统计行数
来源：http://hye.gotoacloud.top

wc -l a.txt
来源：http://xwd.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://tvj.dashuyun.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uvb.yj202588.top

[R54] 比较两个文件
来源：http://rmu.sweek.top

diff a.txt b.txt
来源：http://ika.ydzc1.top

[R55] 压缩与解压
来源：http://mns.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rmm.yonumen.top

[R56] 远程拷贝
来源：http://qqo.iojbl.cn

scp file user@host:/path/
来源：http://ktr.ehwqpu.com

[R57] 远程执行命令
来源：http://vhx.xuanzx.com

ssh user@host 'uptime'
来源：http://fmt.aizwys.cn

[R58] 下载文件
来源：http://yeb.andypj.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pxl.nwbrower.top

[R59] 发 POST JSON
来源：http://pmi.hysaishi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://crz.sjlbkw.cn

[R60] 只看 HTTP 状态码
来源：http://rot.jyoumei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vge.nanxuanxn.top

[R61] 磁盘占用
来源：http://ghm.hnxiangtu.top

df -h;  du -sh *
来源：http://tbd.tanke756.top

[R62] 找最占空间的文件
来源：http://veu.sysykeji.top

du -ah . | sort -rh | head -10
来源：http://gzu.9152youxi.cn

[R63] 内存与进程
来源：http://pmu.sweek.top

free -h;  ps aux | grep nginx
来源：http://lze.yj20258.top

[R64] 结束进程
来源：http://gxn.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://jod.ydjk.org.cn

[R65] 查看端口占用
来源：http://wvr.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mmk.jyoumei.cn

[R66] 定时任务
来源：http://abh.fanxiaobao.xyz

crontab -e;  crontab -l
来源：http://sib.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://bwf.cheryme.top

openssl rand -hex 16
来源：http://dev.wangshuangyany.cn

[R68] 计算文件校验值
来源：http://oki.zhaomingkeji.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://zwq.zdqjudy.top

[R69] 生成随机密码
来源：http://zte.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://gim.bbcook.cn

[R70] 时间戳与互转
来源：http://mfg.tanke756.top

date +%s;  date -d @1700000000
来源：http://qcm.daria6918.cn

[R71] 日期格式化
来源：http://yed.zhongyouzk.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jzk.shzxlz.cn

[R72] 等待端口就绪
来源：http://cne.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fjm.yfazqb.com

[R73] 分割大日志
来源：http://bxj.havefunace.top

split -l 1000 big.log part_
来源：http://ddn.zycfv.cn

[R74] 批量重命名
来源：http://txq.ctjpmb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kwg.jqgufenzy.top

[R75] 导出环境变量
来源：http://sxu.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://gdl.fktsv.cn

[R76] 使用临时文件
来源：http://pxe.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rgj.shanyushiyangtech.top

[R77] 读取用户输入
来源：http://idb.yuxming.cn

read -rp "请输入: " ans
来源：http://tob.wangdashe.top

[R78] 交互式菜单
来源：http://szi.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://hdk.shangyingyoupin.top

[R79] 解析命令行选项
来源：http://qzk.zhoulong.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://opz.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://frt.yonumen.top

time ./run.sh
来源：http://mii.yvedp.cn

================================================================================
来源：http://rkg.pycfn.com

S. C / C++ 专题
来源：http://pis.aibaodan.cn

================================================================================
来源：http://isq.sysykeji.top

[S01] C：Hello World
来源：http://dgd.bbcook.cn

#include <stdio.h>
来源：http://hoe.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://flh.cqqwz.cn

[S02] C：变量与格式化输出
来源：http://bdg.hnxiangtu.top

int a = 10; printf("%d\n", a);
来源：http://fkw.jianghu66.top

[S03] C：读入整数
来源：http://tfb.zdbjq.cn

int x; scanf("%d", &x);
来源：http://qjo.yuxming.cn

[S04] C：字符串复制
来源：http://cgh.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://iyc.guowangkeji.top

[S05] C：字符串长度
来源：http://eyx.hywenlv.cn

strlen(s)
来源：http://anp.fengsongda.top

[S06] C：字符串比较
来源：http://fop.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://vud.hfpthk.cn

[S07] C：数组遍历求和
来源：http://ryo.yfazqb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sjm.guannengcc.top

[S08] C：动态内存分配与释放
来源：http://oor.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://srx.yangfankeji.com

[S09] C：结构体定义与初始化
来源：http://fsq.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://usg.jinqigfzy.top

[S10] C：指针与解引用
来源：http://sem.quarkkingdee.top

int *p = &a;  *p = 5;
来源：http://gqd.ehwqpu.com

[S11] C：逐行读文件
来源：http://gli.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://lmh.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tui.hnxiangtu.top

fclose(f);
来源：http://bwj.zdbjq.cn

[S12] C：写文件
来源：http://wnn.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eye.fengsongda.top

[S13] C：宏定义
来源：http://mkj.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://phh.ehwqpu.com

[S14] C：枚举
来源：http://wwr.uphjek.com

enum Color { RED, GREEN, BLUE };
来源：http://tps.gzhubu.top

[S15] C：类型转换
来源：http://oii.fanxiaobao.xyz

(double) a / b
来源：http://mst.xziqi.cn

[S16] C：位操作置位
来源：http://pse.zdqjudy.top

x |= (1 << 3);
来源：http://hbb.jinyuanbaomall.cn

[S17] C：安全拼接字符串
来源：http://tba.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gzh.sxryk.cn

[S18] C：命令行参数
来源：http://hhr.zhongyouzk.top

int main(int argc, char **argv)
来源：http://zsy.dashuyun.cn

[S19] C：快速排序
来源：http://hwq.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://zxs.zycfv.cn

[S20] C：二分查找
来源：http://wpa.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://amg.sysykeji.top

[S21] C：字符类别判断
来源：http://iuf.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fde.hesvh.cn

[S22] C：字符串转数字
来源：http://ukc.sufxvd.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ybh.nanxinkj.top

[S23] C：随机数
来源：http://dtd.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qej.cheryme.top

[S24] C：获取本地时间
来源：http://boq.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://utm.yongpay.top

[S25] C：内存拷贝
来源：http://fcf.hnxiangtu.top

memcpy(dst, src, n);
来源：http://dxj.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://wrj.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://kdw.jiagoushi.top

[S27] C：定义常量
来源：http://cvy.redwolf501.top

const double PI = 3.14159;
来源：http://ywx.ydjk.org.cn

[S28] C：静态变量
来源：http://qju.chenlongwang.top


<!-- 参考信息 -->