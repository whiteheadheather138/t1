代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fac.pycfn.com

[Q60] 取上一行 / 下一行
来源：http://bel.chenlongwang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lrm.ydjk.org.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://joh.shzxlz.cn

[Q61] 移动平均
来源：http://pmk.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fab.52xcode.cn

[Q62] 分组占比
来源：http://swc.nanxuanxn.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gty.chenlongwang.top

[Q63] 开启事务
来源：http://aju.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://cpd.zhiwuduotai.top

[Q64] 提交事务
来源：http://lkd.gogol.net.cn

COMMIT;
来源：http://lky.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://htn.zhixingplan.top

ROLLBACK;
来源：http://nzb.chenlongwang.top

[Q66] 行锁查询
来源：http://fjj.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gqa.xylfe.cn

[Q67] 设置隔离级别
来源：http://kuj.ywan-chungtsiang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qoq.cucudq.cn

[Q68] 保存点
来源：http://luj.52xcode.cn

SAVEPOINT sp1;
来源：http://nso.ydzc1.top

ROLLBACK TO sp1;
来源：http://rlj.meibo888.top

[Q69] 查看执行计划
来源：http://irm.jianghu66.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jxt.quarkkingdee.top

[Q70] 更新统计信息
来源：http://ntp.fktsv.cn

ANALYZE TABLE users;
来源：http://zht.yfazqb.com

[Q71] 查看建表语句
来源：http://pgy.tanke756.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jja.fengsongda.top

[Q72] 查看索引
来源：http://mnh.ppjwa.cn

SHOW INDEX FROM users;
来源：http://xsu.jlsjyb.cn

[Q73] 查看表状态
来源：http://nqw.shanyushiyangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ujx.fktsv.cn

[Q74] 强制使用索引
来源：http://zte.nwbrower.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mva.svipenyu.cn

[Q75] 日期格式化
来源：http://tbz.iojbl.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fqy.meibo888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zim.yvedp.cn

[Q76] 按天统计
来源：http://fpz.gotoacloud.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://plt.daxiang520.top

[Q77] 时间加减
来源：http://gee.ivvv.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jqu.cqqwz.cn

[Q78] 当前时间
来源：http://uar.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qjz.gotoacloud.top

[Q79] 字符串拼接
来源：http://dcq.zhongyouzk.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ypy.daxiang520.top

[Q80] 字符串截取
来源：http://mxq.chenjidiqi.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vva.chenlongwang.top

[Q81] 字符串替换
来源：http://zox.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://svp.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://zxi.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sbe.uphjek.com

[Q83] 大小写转换
来源：http://jpz.zhengqikj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ajm.iojbl.cn

[Q84] 去除首尾空格
来源：http://lwy.ivvv.top

SELECT TRIM(name) FROM users;
来源：http://dcy.hesvh.cn

[Q85] 数值取整
来源：http://xgv.tianlin.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tmf.yj20258.top

[Q86] 读取 JSON 字段
来源：http://izw.yangfankeji.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hxu.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://jjv.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vgb.jyoumei.cn

[Q88] 行转列（条件聚合）
来源：http://gnf.nanxinkj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gjz.nwbrower.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://shi.zhengqikj.top

[Q89] 判断表是否存在
来源：http://nhn.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rdy.tanke756.top

[Q90] 生成序号列
来源：http://fbq.cheryme.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yjt.jqgufenzy.top

================================================================================
来源：http://heb.hywenlv.cn

R. Bash 专题
来源：http://lrf.xziqi.cn

================================================================================
来源：http://jlh.sufxvd.cn

[R01] shebang 与严格模式
来源：http://dbz.yangfankeji.com

#!/usr/bin/env bash
来源：http://jrl.gzhubu.top

set -euo pipefail
来源：http://bml.gotoacloud.top

[R02] 变量赋值与使用
来源：http://okq.daria6918.cn

name="Tom"; echo "$name"
来源：http://llu.fktsv.cn

[R03] 只读变量
来源：http://xpa.yuanzhike.top

readonly PI=3.14
来源：http://fou.jlsjyb.cn

[R04] 位置参数
来源：http://qcg.xinyue.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pgv.smart0.xyz

[R05] 参数默认值
来源：http://zct.zhongyouzk.top

name="${1:-default}"
来源：http://mxf.ywan-chungtsiang.top

[R06] 判断命令是否存在
来源：http://bvs.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ntq.tanke756.top

[R07] if 判断文件
来源：http://yeh.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mwi.jinyuanbaomall.cn

[R08] 数值比较
来源：http://lzf.yj202588.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rjs.kuanghao11.cn

[R09] 字符串比较
来源：http://zti.yvedp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yyu.zhixingplan.top

[R10] 正则匹配
来源：http://mnn.zhixingplan.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dkc.birdmap.top

[R11] case 多分支
来源：http://fhj.jqgfzy.top

case "$1" in
来源：http://hag.hnqzz.top

start) echo "启动" ;;
来源：http://efr.52xcode.cn

stop)  echo "停止" ;;
来源：http://sug.vqdsnc.cn

*)     echo "未知命令" ;;
来源：http://vrt.epnwcf.com

esac
来源：http://udp.xziqi.cn

[R12] for 遍历文件
来源：http://zye.feifeiyinyue.top

for f in *.txt; do echo "$f"; done
来源：http://alm.hesvh.cn

[R13] for 计数循环
来源：http://vui.havefunace.top

for i in {1..10}; do echo "$i"; done
来源：http://qnn.jiagoushi.top

[R14] C 风格 for
来源：http://wxq.gzhubu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://guy.hysaishi.cn

[R15] while 逐行读文件
来源：http://wgr.hywenlv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rmg.snrcjt.cn

[R16] until 等待条件
来源：http://jug.sweek.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nxi.ybcxt.top

[R17] 数组定义与取值
来源：http://syo.hongshengwenyu.top

arr=(a b c); echo "${arr[0]}"
来源：http://uwy.guannengcc.top

[R18] 遍历数组
来源：http://iis.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xuc.zhengqikj.top

[R19] 数组长度
来源：http://wzc.zdbjq.cn

echo "${#arr[@]}"
来源：http://clj.yonumen.top

[R20] 关联数组（字典）
来源：http://bws.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qfp.aibaodan.cn

[R21] 字符串长度
来源：http://klr.nwbrower.top

echo "${#s}"
来源：http://lve.dianchejie.cn

[R22] 截取子串
来源：http://dtz.yuanzhike.top

echo "${s:0:5}"
来源：http://rmz.yueranfly.top

[R23] 字符串替换
来源：http://zlh.hammf.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ruc.sysykeji.top

[R24] 大小写转换
来源：http://qxn.haohaochexian.top

echo "${s^^}"; echo "${s,,}"
来源：http://ogo.hnxiangtu.top

[R25] 去后缀 / 去前缀
来源：http://yiz.fktsv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mkp.yj20258888.top

[R26] 命令替换
来源：http://yfv.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://qbw.c1oappe.top

[R27] 算术展开
来源：http://wcf.wangshuangyany.cn

echo $((1 + 2 * 3))
来源：http://trb.jinqigufen.top

[R28] 浮点运算
来源：http://tok.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://phx.tanke756.top

[R29] 定义函数
来源：http://fpw.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eng.fengsongda.top

[R30] 函数返回状态码
来源：http://enc.dianchejie.cn

f() { return 0; }; f || echo "失败了"
来源：http://zum.jinqigufen.top

[R31] 局部变量
来源：http://bxo.0kj1m.cn

f() { local x=1; echo "$x"; }
来源：http://mhe.shanyushiyangtech.top

[R32] 参数个数校验
来源：http://qnl.meibo888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://snf.zhengqikj.top

[R33] 捕获错误并提示行号
来源：http://msf.xinyue.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zov.snrcjt.cn

[R34] 退出时清理
来源：http://auy.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://enf.ybcxt.top

[R35] 后台执行并等待
来源：http://vyh.yj202588.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dmy.sweek.top

[R36] 并发执行多个任务
来源：http://rxx.9152youxi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zib.sysykeji.top

[R37] 把输出赋给变量
来源：http://kuf.ybcxt.top

files=$(ls -1)
来源：http://xnn.ydjk.org.cn

[R38] 管道串联
来源：http://eko.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://iqx.chenlongwang.top

[R39] 重定向标准输出与错误
来源：http://oug.jianghu66.top

cmd > out.log 2>&1
来源：http://ybn.xuanzx.com

[R40] 追加写日志
来源：http://mvc.gaohongyu789.top

echo "log" >> out.log
来源：http://fbl.nanxuanxn.top

[R41] 丢弃输出
来源：http://ifs.cashguo.top

cmd >/dev/null 2>&1
来源：http://tib.feifeiyinyue.top

[R42] 输入重定向
来源：http://sqf.c1oappe.top

wc -l < a.txt
来源：http://bts.chenjidiqi.icu

[R43] 按名字查找文件
来源：http://uhe.ydzc1.top

find . -name "*.log" -type f
来源：http://nms.ivvv.top

[R44] 按修改时间查找
来源：http://xcp.chenjidiqi.icu

find . -mtime -7 -type f
来源：http://cwy.316326.xyz

[R45] 批量删除
来源：http://wdw.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://yhl.andypj.xyz

[R46] 递归替换文件内容
来源：http://jbb.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vud.sysykeji.top

[R47] sed 单行替换
来源：http://jmq.hongshengwenyu.top

sed -i 's/foo/bar/g' a.txt
来源：http://xcd.zhiwuduotai.top

[R48] awk 取指定列
来源：http://ubm.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://oit.vqdsnc.cn

[R49] awk 带条件
来源：http://nnt.yanxiufei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yff.zdbjq.cn

[R50] awk 求和
来源：http://qps.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xja.havefunace.top

[R51] 排序去重取前几
来源：http://nvf.feifeiyinyue.top

sort a.txt | uniq -c | sort -rn | head
来源：http://urb.ydzc1.top

[R52] 统计行数
来源：http://pyl.52xcode.cn

wc -l a.txt
来源：http://ahn.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://akh.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aci.ydjk.org.cn

[R54] 比较两个文件
来源：http://nqn.jlsjyb.cn

diff a.txt b.txt
来源：http://wzo.9152youxi.cn

[R55] 压缩与解压
来源：http://wdi.cqqwz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kch.meibo888.top

[R56] 远程拷贝
来源：http://hgp.nwbrower.top

scp file user@host:/path/
来源：http://sua.pycfn.com

[R57] 远程执行命令
来源：http://vkv.cheryme.top

ssh user@host 'uptime'
来源：http://tru.zhoulong.xyz

[R58] 下载文件
来源：http://eac.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bfn.jqgfzy.top

[R59] 发 POST JSON
来源：http://vlt.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jjn.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://ioz.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vqh.yuxming.cn

[R61] 磁盘占用
来源：http://fgq.quarkkingdee.top

df -h;  du -sh *
来源：http://oxo.wangdashe.top

[R62] 找最占空间的文件
来源：http://gvp.mhx1999.top

du -ah . | sort -rh | head -10
来源：http://cao.xuetiantiany.cn

[R63] 内存与进程
来源：http://ssb.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://kbb.yanxiufei.cn

[R64] 结束进程
来源：http://xas.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://fxk.hesvh.cn

[R65] 查看端口占用
来源：http://ivn.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hed.xinyue.icu

[R66] 定时任务
来源：http://fmq.ybcxt.top

crontab -e;  crontab -l
来源：http://kdu.yuanzhike.top

[R67] 生成随机十六进制串
来源：http://rck.cheryme.top

openssl rand -hex 16
来源：http://xvx.kuanghao11.cn

[R68] 计算文件校验值
来源：http://ksr.zycfv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vxt.shanyushiyangtech.top

[R69] 生成随机密码
来源：http://yea.hywenlv.cn

head -c 16 /dev/urandom | base64
来源：http://nxp.zhaomingkeji.xyz

[R70] 时间戳与互转
来源：http://srw.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://jdx.cucudq.cn

[R71] 日期格式化
来源：http://xzk.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://swl.pycfn.com

[R72] 等待端口就绪
来源：http://opk.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rhp.zhoulong.xyz

[R73] 分割大日志
来源：http://oev.316326.xyz

split -l 1000 big.log part_
来源：http://qhu.cqqwz.cn

[R74] 批量重命名
来源：http://yqd.xylfe.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uvr.yueranfly.top

[R75] 导出环境变量
来源：http://sho.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://ovw.nanxinkj.top

[R76] 使用临时文件
来源：http://neu.iojbl.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uwr.vqdsnc.cn

[R77] 读取用户输入
来源：http://pjt.shanyushiyangkeji.top

read -rp "请输入: " ans
来源：http://yic.smart0.xyz

[R78] 交互式菜单
来源：http://vyh.uphjek.com

select opt in a b c; do echo "$opt"; break; done
来源：http://cly.guannengcc.top

[R79] 解析命令行选项
来源：http://wti.xuanzx.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rhw.feifeiyinyue.top

[R80] 查看脚本执行耗时
来源：http://lfc.gaohongyu789.top

time ./run.sh
来源：http://lmu.jqgufenzy.top

================================================================================
来源：http://byt.quarkkingdee.top

S. C / C++ 专题
来源：http://ghq.chenzaomai.com

================================================================================
来源：http://cgm.yueranfly.top

[S01] C：Hello World
来源：http://rsu.c1oappe.top

#include <stdio.h>
来源：http://gjq.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uxk.fengsongda.top

[S02] C：变量与格式化输出
来源：http://trh.ywan-chungtsiang.top

int a = 10; printf("%d\n", a);
来源：http://ujq.daria6918.cn

[S03] C：读入整数
来源：http://kqt.jqgfzy.top

int x; scanf("%d", &x);
来源：http://gmz.yj20258.top

[S04] C：字符串复制
来源：http://okn.chenlongwang.top

char dst[32]; strcpy(dst, "hi");
来源：http://xlc.gaohongyu789.top

[S05] C：字符串长度
来源：http://eot.jiagoushi.top

strlen(s)
来源：http://xny.aizwys.cn

[S06] C：字符串比较
来源：http://hbw.jianghu66.top

strcmp(a, b) == 0
来源：http://dht.hnxiangtu.top

[S07] C：数组遍历求和
来源：http://qmf.0kj1m.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ycs.xziqi.cn

[S08] C：动态内存分配与释放
来源：http://jgj.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kom.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://ecw.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://onm.andypj.xyz

[S10] C：指针与解引用
来源：http://ltr.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://clx.dianchejie.cn

[S11] C：逐行读文件
来源：http://ewd.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://agr.jianghu66.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kvy.zhengqikj.top

fclose(f);
来源：http://zhg.jinqigufen.top

[S12] C：写文件
来源：http://jpt.jinghuilouyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tkv.meibo888.top

[S13] C：宏定义
来源：http://nsg.hnxiangtu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jrv.hysaishi.cn

[S14] C：枚举
来源：http://oas.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://gvp.gotoacloud.top

[S15] C：类型转换
来源：http://wbg.redwolf501.top

(double) a / b
来源：http://hme.pycfn.com

[S16] C：位操作置位
来源：http://gyp.cucudq.cn

x |= (1 << 3);
来源：http://cnn.hammf.cn

[S17] C：安全拼接字符串
来源：http://hlx.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zmy.haohaochexian.top

[S18] C：命令行参数
来源：http://foq.xylfe.cn

int main(int argc, char **argv)
来源：http://ljt.jlsjyb.cn

[S19] C：快速排序
来源：http://dlv.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://dcr.hongshengwenyu.top

[S20] C：二分查找
来源：http://pju.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://awt.ydjk.org.cn

[S21] C：字符类别判断
来源：http://she.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ffc.nanxuanxn.top

[S22] C：字符串转数字
来源：http://ahs.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://dzd.52xcode.cn

[S23] C：随机数
来源：http://cjg.shanyushiyangtech.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yuh.nanxinkj.top

[S24] C：获取本地时间
来源：http://fsj.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dys.ydzc1.top

[S25] C：内存拷贝
来源：http://jde.zhaomingkeji.xyz

memcpy(dst, src, n);
来源：http://njb.cucudq.cn

[S26] C：内存清零
来源：http://iqk.meibo888.top

memset(a, 0, sizeof a);
来源：http://ooo.hongshengwenyu.top

[S27] C：定义常量
来源：http://nsu.yuxming.cn

const double PI = 3.14159;
来源：http://kec.fktsv.cn

[S28] C：静态变量
来源：http://crd.birdmap.top

static int counter = 0;
来源：http://arn.gaohongyu789.top

[S29] C：变参函数
来源：http://bgp.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mxo.svipenyu.cn

[S30] C：头文件保护
来源：http://crz.aizwys.cn


<!-- 参考信息 -->